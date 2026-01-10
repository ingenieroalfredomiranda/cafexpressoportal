<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</title>
  <meta name="description" content="Investigación especial — Café Expresso Portal. La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras en Culiacán." />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#A61B1B;
      --blue:#0B3D91;
      --muted:#4A4A4A;
      --white:#ffffff;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:'Inter',system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;color:#222;background:#fff;line-height:1.45}
    /* HERO */
    .hero-article{position:relative;width:100%;height:62vh;min-height:420px;overflow:hidden;display:block;cursor:pointer;padding-bottom:18px}
    .hero-img{width:100%;height:100%;object-fit:cover;display:block;transition:opacity .35s ease;z-index:0}
    .hero-overlay{position:absolute;inset:0;background:linear-gradient(135deg, rgba(11,61,145,0.55) 0%, rgba(0,0,0,0.25) 60%);pointer-events:none;z-index:1}
    /* Texto del hero desplazado hacia abajo ~3-4 renglones */
    .hero-text{position:absolute;top:24%;left:6%;right:6%;color:var(--white);text-shadow:0 6px 18px rgba(0,0,0,0.55);max-width:58%;z-index:2;max-height:70%;overflow:auto;padding-right:8px}
    .hero-title{margin:0 0 12px 0;font-weight:800;line-height:1.02;font-size:clamp(28px,4.6vw,56px);letter-spacing:-0.02em;word-break:break-word;overflow-wrap:break-word}
    .hero-sub{margin:0;font-weight:500;font-size:clamp(13px,1.6vw,20px);opacity:0.98;word-break:break-word;overflow-wrap:break-word}
    .hero-credit{position:absolute;right:4%;bottom:3%;font-size:12px;color:rgba(255,255,255,0.95);text-shadow:0 2px 6px rgba(0,0,0,0.6);z-index:3}

    /* Contenido principal */
    .container{max-width:1100px;margin:28px auto;padding:0 20px; margin-top:-40px;} /* sube todo el bloque principal */
    .kicker{color:var(--muted);font-weight:600;margin-bottom:8px;margin-top:-18px;display:inline-block;line-height:1} /* pega "Investigación" con el renglón superior */
    .lead{font-size:18px;color:#111;margin:12px 0 20px;margin-top:-24px} /* sube el párrafo principal para eliminar hueco */
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
    button{cursor:pointer}

    @media (max-width:980px){
      .two-col{grid-template-columns:1fr}
      .hero-text{max-width:86%}
    }
    @media (max-width:600px){
      .hero-article{height:48vh;min-height:320px}
      .hero-title{font-size:clamp(20px,7.5vw,32px)}
      .hero-sub{font-size:14px}
      /* en móviles se reduce el desplazamiento para que el texto no quede demasiado abajo */
      .hero-text{top:16%;left:6%;right:6%}
      .hero-credit{left:6%;right:auto;bottom:6%}
      .container{margin-top:-18px}
      .lead{margin-top:-12px}
      .kicker{margin-top:-8px}
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
    </div>

    <div class="hero-credit">Crédito foto: Investigaciones Café Expresso Portal</div>
  </header>

  <main class="container" id="maincontent">
    <div class="kicker">Investigación</div>

    <article>
      <p class="lead">“La máquina me decía que la próxima vez recuperaría todo. Perdí la casa, la dignidad y casi la vida.” Ese testimonio, recogido entre exjugadores de Culiacán, resume la progresión que convierte el ocio en urgencia. Esta investigación cruza relatos personales, documentos y datos para mostrar por qué la ludopatía ya no es solo un problema privado sino una crisis pública en Sinaloa.</p>

      <div class="two-col">
        <div>
          <h2>Contexto y antecedentes</h2>
          <p>En la última década la oferta de juego en Sinaloa se multiplicó: salas de juego, minicasinos y plataformas digitales que facilitan apuestas desde el teléfono. La combinación de accesibilidad, falta de controles y redes financieras opacas ha creado un ecosistema donde el riesgo social se amplifica.</p>

          <h2>Galería y subida de imágenes</h2>
          <p class="small">Puedes subir imágenes relacionadas con la investigación. Las imágenes se guardan en el servidor y se muestran en la galería.</p>

          <form id="uploadForm" class="upload-form" action="/upload" method="post" enctype="multipart/form-data">
            <input id="fileInput" type="file" name="imagen" accept="image/*" required>
            <button type="submit">Subir</button>
          </form>

          <div id="mensaje" aria-live="polite"></div>
          <div class="galeria" id="galeria"></div>
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
    // Lista final de imágenes solicitada (sin "image48")
    const imageFiles = [
      'imagen2.webp',
      'imagen3.webp',
      'imagen4.webp',
      'imagen5.webp',
      'imagen31.webp',
      'imagen41.webp'
    ];

    (function initGallery() {
      const heroImg = document.getElementById('heroImg');
      const thumbs = document.getElementById('thumbs');
      const gal = document.getElementById('galeria');

      if (!imageFiles.length) {
        thumbs.innerHTML = '<div class="small">No hay miniaturas configuradas.</div>';
        heroImg.src = '';
        return;
      }

      // Establecer la primera imagen como portada inicial
      heroImg.src = imageFiles[0];

      // Crear miniaturas y poblar galería
      imageFiles.forEach((name, idx) => {
        // miniatura
        const t = document.createElement('img');
        t.src = name;
        t.alt = 'Miniatura ' + (idx + 1);
        t.dataset.src = name;
        if (idx === 0) t.classList.add('selected');
        t.addEventListener('click', () => {
          thumbs.querySelectorAll('img').forEach(x => x.classList.remove('selected'));
          t.classList.add('selected');
          heroImg.src = t.dataset.src;
        });
        thumbs.appendChild(t);

        // galería inferior
        const g = document.createElement('img');
        g.src = name;
        g.alt = 'Galería ' + (idx + 1);
        gal.appendChild(g);
      });
    })();

    // Subida AJAX con fallback
    (function() {
      const form = document.getElementById('uploadForm');
      const fileInput = document.getElementById('fileInput');
      const mensaje = document.getElementById('mensaje');
      const gal = document.getElementById('galeria');

      form.addEventListener('submit', async (e) => {
        e.preventDefault();
        mensaje.innerHTML = '';
        const file = fileInput.files[0];
        if (!file) return;
        const fd = new FormData();
        fd.append('imagen', file);

        try {
          const res = await fetch('/upload-ajax', { method: 'POST', body: fd });
          if (!res.ok) {
            if (res.status === 404) { form.removeEventListener('submit', arguments.callee); form.submit(); return; }
            const err = await res.json().catch(()=>({ error: 'Error al subir' }));
            throw new Error(err.error || 'Error al subir');
          }
          const json = await res.json();
          if (!json.filename) throw new Error('Respuesta inválida del servidor');
          const img = document.createElement('img');
          img.src = '/uploads/' + encodeURIComponent(json.filename);
          gal.prepend(img);
          mensaje.innerHTML = '<div class="msg ok">Imagen subida correctamente.</div>';
          form.reset();
        } catch (err) {
          mensaje.innerHTML = '<div class="msg err">' + (err.message || 'Error al subir') + '</div>';
        }
      });
    })();
  </script>
</body>
</html>




