<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#A61B1B;
      --blue:#0B3D91;
      --muted:#4A4A4A;
      --white:#ffffff;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:'Inter',system-ui,-apple-system,Segoe UI,Roboto,Arial;color:#222;background:#fff;line-height:1.45}

    /* HERO: reducir altura en lugar de mover el contenido principal con márgenes negativos.
       Esto evita que la información "de abajo" se pierda o se superponga. */
    .hero-article{
      position:relative;
      width:100%;
      height:56vh;           /* altura ligeramente menor para dejar más espacio al contenido */
      min-height:360px;
      overflow:hidden;
      display:block;
      cursor:pointer;
      padding-bottom:0;
      background:#111;
    }
    .hero-img{width:100%;height:100%;object-fit:cover;display:block;transition:opacity .35s ease;z-index:0}
    .hero-overlay{position:absolute;inset:0;background:linear-gradient(135deg, rgba(11,61,145,0.55) 0%, rgba(0,0,0,0.25) 60%);pointer-events:none;z-index:1}

    /* Ajuste del texto dentro del hero: bajar el texto sin tocar el flujo del main */
    .hero-text{
      position:absolute;
      top:26%;               /* controla cuánto baja el texto dentro del hero */
      left:6%;
      right:6%;
      color:var(--white);
      text-shadow:0 6px 18px rgba(0,0,0,0.55);
      max-width:58%;
      z-index:2;
      overflow:auto;
      padding-right:8px;
    }
    .hero-title{margin:0 0 12px 0;font-weight:800;line-height:1.02;font-size:clamp(28px,4.6vw,56px);letter-spacing:-0.02em}
    .hero-sub{margin:0;font-weight:500;font-size:clamp(13px,1.6vw,20px);opacity:0.98}
    .hero-credit{position:absolute;right:4%;bottom:3%;font-size:12px;color:rgba(255,255,255,0.95);z-index:3}

    /* CONTENIDO PRINCIPAL: quitar márgenes negativos y usar padding para separación segura */
    .container{
      max-width:1100px;
      margin:28px auto;
      padding:0 20px 48px 20px; /* padding-bottom para que el contenido final no quede pegado al borde */
      margin-top:0;             /* importante: no usar valores negativos aquí */
    }
    .kicker{color:var(--muted);font-weight:600;margin-bottom:8px;display:inline-block;line-height:1}
    .lead{font-size:18px;color:#111;margin:8px 0 20px} /* margen normal: no negativo */
    .meta{color:var(--muted);font-size:13px;margin-bottom:18px}
    h2{font-size:22px;margin:22px 0 12px}
    p{margin:0 0 14px}
    .two-col{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:start}
    .sidebar{background:#fafafa;padding:18px;border-radius:8px;border:1px solid #eee}
    .recuadro{background:#fff;border-left:4px solid var(--accent);padding:12px 14px;margin:14px 0;border-radius:4px}
    .pull{font-weight:700;font-size:20px;color:#111;margin:18px 0}
    .small{font-size:13px;color:var(--muted)}
    .toggle-hint{font-size:12px;color:rgba(255,255,255,0.9);margin-top:8px;opacity:0.95}

    /* Miniaturas y galería */
    .thumbs{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
    .thumbs img{width:110px;height:70px;object-fit:cover;border-radius:6px;border:2px solid transparent;cursor:pointer}
    .thumbs img.selected{border-color:var(--accent)}
    .galeria{display:flex;flex-wrap:wrap;margin-top:12px}
    .galeria img{max-width:220px;margin:8px;border-radius:6px;border:1px solid #e6e6e6}
    .msg{padding:10px;border-radius:6px;margin-top:12px}
    .msg.ok{background:#e6ffed;border:1px solid #bff0c9;color:#064d1a}
    .msg.err{background:#ffecec;border:1px solid #ffbdbd;color:#6b0000}
    .diagnostic{font-size:13px;color:var(--muted);margin-top:8px}

    @media (max-width:980px){
      .two-col{grid-template-columns:1fr}
      .hero-text{max-width:86%}
    }
    @media (max-width:600px){
      .hero-article{height:48vh;min-height:320px}
      .hero-title{font-size:clamp(20px,7.5vw,32px)}
      .hero-sub{font-size:14px}
      .hero-text{top:16%} /* en móviles bajar menos para que no tape contenido */
      .container{margin-top:0;padding-bottom:36px}
    }
    @media (max-width:420px){
      .hero-text{max-width:92%;max-height:72%}
      .hero-title{font-size:18px;line-height:1.05}
      .hero-sub{font-size:13px}
      .hero-credit{bottom:6%;right:6%;font-size:11px}
    }
    a:focus{outline:3px solid var(--blue);outline-offset:2px}
  </style>
</head>
<body>
  <!-- HERO -->
  <header id="hero" class="hero-article" role="img" aria-label="Portada de investigación">
    <img id="heroImg" src="" alt="Portada principal" class="hero-img" />
    <div class="hero-overlay" aria-hidden="true"></div>

    <div class="hero-text">
      <h1 class="hero-title">Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</h1>
      <p class="hero-sub"><strong>Investigación especial — Café Expresso Portal | Culiacán, Sinaloa</strong><br><em>La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras.</em></p>
      <div class="toggle-hint" id="toggleHint">Selecciona una miniatura para cambiar la portada</div>
      <div class="thumbs" id="thumbs" aria-hidden="false"></div>
      <div id="diagnostic" class="diagnostic" aria-live="polite"></div>
    </div>

    <div class="hero-credit">Crédito foto: Investigaciones Café Expresso Portal</div>
  </header>

  <main class="container" id="maincontent">
    <div class="kicker">Investigación</div>

    <article>
      <!-- Párrafo principal: ya no subimos con márgenes negativos para evitar solapamiento -->
      <p class="lead">“La máquina me decía que la próxima vez recuperaría todo. Perdí la casa, la dignidad y casi la vida.” Ese testimonio, recogido entre exjugadores de Culiacán, resume la progresión que convierte el ocio en urgencia. Esta investigación cruza relatos personales, documentos y datos para mostrar por qué la ludopatía ya no es solo un problema privado sino una crisis pública en Sinaloa.</p>

      <div class="two-col">
        <div>
          <h2>Contexto y antecedentes</h2>
          <p>En la última década la oferta de juego en Sinaloa se multiplicó: salas de juego, minicasinos y plataformas digitales que facilitan apuestas desde el teléfono. La combinación de accesibilidad, falta de controles y redes financieras opacas ha creado un ecosistema donde el riesgo social se amplifica.</p>

          <h2>Galería</h2>
          <p class="small">Las imágenes encontradas en la carpeta se muestran abajo; si no aparecen, revisa nombres y rutas.</p>
          <div class="galeria" id="galeria"></div>

          <h2>Lecturas recomendadas</h2>
          <div class="recuadro">
            <p class="pull">Vacíos regulatorios y apuestas digitales</p>
            <p class="small">Un repaso a cómo la normativa no ha seguido el ritmo de la tecnología y qué implica para comunidades vulnerables.</p>
          </div>

          <h2>Hallazgos principales</h2>
          <p>Un problema multicausal y en crecimiento. La ludopatía combina factores individuales, sociales y tecnológicos. Estudios sitúan la prevalencia entre 1% y 3% de la población.</p>

          <h2>Si te identificas</h2>
          <p class="small"><strong>Señales:</strong> priorizar apuestas; mentir sobre tiempo o dinero; pedir prestado; uso compulsivo de tarjetas; aislamiento; cambios de humor; intentos autolesivos.</p>
          <p class="small"><strong>Qué hacer:</strong> detener depósitos; conservar comprobantes; bloquear tarjetas; buscar ayuda en salud mental o grupos de apoyo; solicitar autexclusión si está disponible.</p>
        </div>

        <aside class="sidebar" aria-labelledby="sidebarTitle">
          <h3 id="sidebarTitle">Datos clave</h3>
          <p class="small">Prevalencia estimada: 1%–3% de la población; Riesgo de suicidio: hasta 15 veces mayor en personas con ludopatía.</p>
          <div class="recuadro">
            <strong>Contacto:</strong>
            <p class="small">Redacción — Café Expresso Portal</p>
          </div>
        </aside>
      </div>
    </article>
  </main>

  <script>
    /* Robust image loader:
       - prueba varias extensiones para cada base de nombre
       - usa la primera encontrada como portada
       - no modifica el flujo del documento (no hay márgenes negativos)
       - muestra diagnóstico en la página y en consola
    */
    const imageBases = ['imagen2','imagen3','imagen4','imagen5','imagen31','imagen41'];
    const exts = ['.webp','.avif','.jpg','.jpeg','.png'];
    const PLACEHOLDER = 'data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///ywAAAAAAQABAAACAUwAOw==';
    const diagEl = document.getElementById('diagnostic');

    function logConsole(msg){ console.log('[PORTADA] ' + msg); if (diagEl) diagEl.textContent = msg; }

    function testImage(url, timeout = 3000){
      return new Promise(resolve => {
        const img = new Image();
        let done = false;
        const timer = setTimeout(() => { if (!done){ done = true; resolve(false); img.src = ''; } }, timeout);
        img.onload = () => { if (!done){ done = true; clearTimeout(timer); resolve(true); } };
        img.onerror = () => { if (!done){ done = true; clearTimeout(timer); resolve(false); } };
        img.src = url;
      });
    }

    async function resolvePaths(bases, extensions){
      const results = [];
      for (const base of bases){
        let found = null;
        for (const ext of extensions){
          const candidate = base + ext;
          try {
            const ok = await testImage(candidate);
            if (ok){ found = candidate; logConsole('Encontrada: ' + candidate); break; }
            else logConsole('No encontrada: ' + candidate);
          } catch(e){
            logConsole('Error probando ' + candidate + ': ' + e);
          }
        }
        results.push(found);
      }
      return results;
    }

    async function init(){
      diagEl && (diagEl.textContent = 'Buscando imágenes en la carpeta...');
      const resolved = await resolvePaths(imageBases, exts);
      const heroImg = document.getElementById('heroImg');
      const thumbs = document.getElementById('thumbs');
      const gal = document.getElementById('galeria');

      thumbs.innerHTML = '';
      gal.innerHTML = '';

      const firstValid = resolved.find(p => p);
      if (firstValid){
        heroImg.src = firstValid;
        heroImg.onerror = () => { heroImg.src = PLACEHOLDER; logConsole('Error cargando portada: ' + firstValid); };
        logConsole('Portada establecida: ' + firstValid);
      } else {
        heroImg.src = PLACEHOLDER;
        logConsole('No se encontraron imágenes válidas. Revisa nombres y rutas.');
      }

      resolved.forEach((path, idx) => {
        const thumb = document.createElement('img');
        thumb.alt = 'Miniatura ' + (idx + 1);
        thumb.src = path || PLACEHOLDER;
        thumb.dataset.src = path || '';
        thumb.addEventListener('click', () => {
          if (thumb.dataset.src){
            heroImg.src = thumb.dataset.src;
            thumbs.querySelectorAll('img').forEach(x => x.classList.remove('selected'));
            thumb.classList.add('selected');
            logConsole('Portada cambiada: ' + thumb.dataset.src);
          }
        });
        if (idx === 0) thumb.classList.add('selected');
        thumbs.appendChild(thumb);

        const g = document.createElement('img');
        g.alt = 'Galería ' + (idx + 1);
        g.src = path || PLACEHOLDER;
        gal.appendChild(g);
      });

      // resumen en consola
      logConsole('Resumen de imágenes:');
      resolved.forEach((p,i) => logConsole(imageBases[i] + ' -> ' + (p || 'NO ENCONTRADA')));
    }

    document.addEventListener('DOMContentLoaded', () => {
      init().catch(err => {
        console.error('[PORTADA] Error inicializando:', err);
        diagEl && (diagEl.textContent = 'Error al inicializar la galería. Revisa la consola.');
      });
    });
  </script>
</body>
</html>





