

<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</title>
  <meta name="description" content="Investigación especial — Café Expresso Portal. La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras en Culiacán." />
  <meta property="og:title" content="Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa" />
  <meta property="og:description" content="Investigación especial — Café Expresso Portal. La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras en Culiacán." />
  <meta property="og:type" content="article" />
  <meta property="og:image" content="https://ingenieroalfredomiranda.github.io/cafexpressosportal/apuestas.jpg" />
  <meta property="og:site_name" content="Café Expresso Portal" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#A61B1B;
      --blue:#0B3D91;
      --muted:#4A4A4A;
      --white:#ffffff;
      --hero-height:62vh; /* Ajusta si cambias la altura del hero */
      --hero-gap:20px;    /* Espacio entre hero y contenido */
    }

    *{box-sizing:border-box}
    body{margin:0;font-family:'Inter',system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;color:#222;background:#fff;line-height:1.45}

    /* HERO */
    .hero-article{
      position:relative;
      width:100%;
      height:var(--hero-height);
      min-height:420px;
      overflow:hidden;
      display:block;
      cursor:pointer;
    }
    .hero-img{width:100%;height:100%;object-fit:cover;display:block;transition:opacity .35s ease}
    .hero-overlay{position:absolute;inset:0;background:linear-gradient(135deg, rgba(11,61,145,0.55) 0%, rgba(0,0,0,0.25) 60%);pointer-events:none}
    .hero-text{position:absolute;top:6%;left:6%;right:6%;color:var(--white);text-shadow:0 6px 18px rgba(0,0,0,0.55);max-width:58%}
    .hero-title{margin:0 0 12px 0;font-weight:800;line-height:1.02;font-size:clamp(28px,4.6vw,56px);letter-spacing:-0.02em}
    .hero-sub{margin:0;font-weight:500;font-size:clamp(13px,1.6vw,20px);opacity:0.98}
    .hero-credit{position:absolute;right:4%;bottom:3%;font-size:12px;color:rgba(255,255,255,0.95);text-shadow:0 2px 6px rgba(0,0,0,0.6)}

    /* MAIN: padding-top evita solapamiento con el hero */
    .container{
      max-width:1100px;
      margin:0 auto;
      padding:calc(var(--hero-height) + var(--hero-gap)) 20px 48px;
    }

    .kicker{color:var(--muted);font-weight:600;margin-bottom:8px}
    .lead{font-size:18px;color:#111;margin:12px 0 20px}
    .meta{color:var(--muted);font-size:13px;margin-bottom:18px}
    h2{font-size:22px;margin:22px 0 12px}
    p{margin:0 0 14px}
    .two-col{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:start}
    .sidebar{background:#fafafa;padding:18px;border-radius:8px;border:1px solid #eee}
    .recuadro{background:#fff;border-left:4px solid var(--accent);padding:16px 14px;margin:18px 0;border-radius:6px;position:relative;z-index:2;box-shadow:0 6px 18px rgba(0,0,0,0.06)}
    .pull{font-weight:700;font-size:20px;color:#111;margin:18px 0}
    .small{font-size:13px;color:var(--muted)}

    /* Galería y miniaturas */
    .gallery{display:flex;gap:10px;flex-wrap:wrap;margin-top:18px}
    .thumb{width:120px;height:80px;object-fit:cover;border-radius:6px;border:1px solid #e6e6e6;cursor:pointer;transition:transform .15s ease,box-shadow .15s ease}
    .thumb:focus{outline:3px solid var(--blue);outline-offset:2px}
    .thumb:hover{transform:translateY(-4px);box-shadow:0 8px 20px rgba(0,0,0,0.12)}
    .hero-controls{display:flex;gap:8px;align-items:center;margin-top:10px}
    .btn{background:rgba(255,255,255,0.12);color:var(--white);border:1px solid rgba(255,255,255,0.12);padding:8px 10px;border-radius:6px;font-weight:600;cursor:pointer}
    .btn:focus{outline:3px solid var(--blue);outline-offset:2px}

    /* Responsive */
    @media (max-width:980px){
      .two-col{grid-template-columns:1fr}
      .hero-text{max-width:86%}
    }
    @media (max-width:600px){
      :root{ --hero-height:48vh; }
      .container{ padding:calc(var(--hero-height) + 14px) 16px 32px; }
      .hero-article{height:var(--hero-height);min-height:320px}
      .hero-title{font-size:clamp(20px,7.5vw,32px)}
      .hero-sub{font-size:14px}
      .hero-text{top:8%;left:6%;right:6%}
      .hero-credit{left:6%;right:auto;bottom:6%}
      .thumb{width:72px;height:48px}
    }

    a:focus{outline:3px solid var(--blue);outline-offset:2px}
  </style>
</head>
<body>
  <header id="hero" class="hero-article" role="img" aria-label="Portada de investigación: fachada de casino iluminada en Culiacán con silueta humana en primer plano.">
    <img id="heroImg" src="apuestas.jpg" alt="Fachada de casino iluminada en Culiacán con neón; silueta de una persona en primer plano y reflejos en pavimento húmedo" class="hero-img" />
    <div class="hero-overlay" aria-hidden="true"></div>

    <div class="hero-text">
      <h1 class="hero-title">Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</h1>
      <p class="hero-sub"><strong>Investigación especial — Café Expresso Portal | Culiacán, Sinaloa</strong><br><em>La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras.</em></p>
      <div class="hero-controls" aria-hidden="false">
        <button id="prevBtn" class="btn" aria-label="Imagen anterior">Anterior</button>
        <button id="nextBtn" class="btn" aria-label="Siguiente imagen">Siguiente</button>
      </div>
    </div>

    <div class="hero-credit">Crédito foto: Investigaciones Café Expresso Portal</div>
  </header>

  <main class="container" id="maincontent">
    <div class="kicker">Investigación</div>
    <article>
      <p class="lead">“La máquina me decía que la próxima vez recuperaría todo. Perdí la casa, la dignidad y casi la vida.” Ese testimonio, recogido entre exjugadores de Culiacán, resume la progresión que convierte el ocio en urgencia. Esta investigación cruza relatos personales, documentos y datos para mostrar por qué la ludopatía ya no es solo un problema privado sino una crisis pública en Sinaloa.</p>

      <div class="two-col">
        <div>
          <h2>Galería de imágenes</h2>
          <p class="small">Haz clic en una miniatura para que aparezca como portada principal.</p>

          <div class="gallery" id="gallery">
            <img class="thumb" data-src="apuestas.jpg" src="apuestas.jpg" alt="Portada 1 — apuestas" tabindex="0" />
            <img class="thumb" data-src="apuestas2.jpg" src="apuestas2.jpg" alt="Portada 2 — apuestas2" tabindex="0" />
            <img class="thumb" data-src="portada-v2.jpg" src="portada-v2.jpg" alt="Portada v2" tabindex="0" />
            <img class="thumb" data-src="imagen2.webp.png" src="imagen2.webp.png" alt="Imagen 2" tabindex="0" />
            <img class="thumb" data-src="imagen3.webp.jpg" src="imagen3.webp.jpg" alt="Imagen 3" tabindex="0" />
            <img class="thumb" data-src="imagen31.webp.jpg" src="imagen31.webp.jpg" alt="Imagen 31" tabindex="0" />
            <img class="thumb" data-src="imagen41.webp.avif" src="imagen41.webp.avif" alt="Imagen 41" tabindex="0" />
            <img class="thumb" data-src="imagen5.webp.png" src="imagen5.webp.png" alt="Imagen 5" tabindex="0" />
          </div>

          <h2>Contexto y antecedentes</h2>
          <p>En la última década la oferta de juego en Sinaloa se multiplicó: salas de juego, minicasinos y plataformas digitales se expandieron en zonas urbanas y rurales. Reportes periodísticos, testimonios y acciones de autoridad muestran una doble crisis: salud pública por el aumento de conductas adictivas y vulnerabilidades regulatorias que facilitan opacidad financiera.</p>

          <h2>Hallazgos principales</h2>
          <p><strong>Un problema multicausal y en crecimiento.</strong> La ludopatía combina factores individuales, sociales y tecnológicos. Estudios sitúan la prevalencia entre 1% y 3% de la población, lo que convierte al fenómeno en un problema de salud pública con impacto familiar y comunitario.</p>

          <p><strong>Diseño y accesibilidad que favorecen la dependencia.</strong> Máquinas, minicasinos y plataformas digitales comparten mecanismos de refuerzo intermitente y estímulos sensoriales que aceleran la repetición de la conducta.</p>

          <p><strong>Señales de opacidad financiera.</strong> Inspecciones y aseguramientos en establecimientos de Sinaloa, junto con anuncios de la UIF y la Presidencia sobre revisión de permisos, apuntan a vulnerabilidades regulatorias que pueden facilitar operaciones irregulares y lavado de dinero. Hasta obtener carpetas oficiales, estas vinculaciones se presentan como <em>presuntas</em>.</p>

          <h2>Metodología</h2>
          <p><strong>Enfoque mixto.</strong> Entrevistas semiestructuradas con 18 fuentes; observación en 12 puntos de apuestas; revisión de 34 notas y comunicados; solicitudes formales a UIF, FGR, Fiscalía estatal, Salud Sinaloa y Segob. Cada afirmación clave fue contrastada con al menos dos fuentes independientes. Identidades protegidas y cadena de custodia para documentos sensibles.</p>

          <div class="recuadro">
            <strong>Verificación y transparencia</strong>
            <p class="small">Solicitudes formales enviadas para carpetas de investigación, actas de aseguramiento, cifras de atención 2021–2024 y borrador de la reforma a la Ley de Juegos y Sorteos. Café Expresso Portal publicará íntegros los documentos recibidos.</p>
          </div>

          <h2>Recomendaciones</h2>
          <p><strong>Para autoridades:</strong> límites por defecto, autoexclusión obligatoria, auditorías AML públicas y financiamiento para plazas de tratamiento.</p>
          <p><strong>Para operadores:</strong> políticas verificables de responsabilidad social y protocolos de derivación a servicios de salud.</p>
          <p><strong>Para la prensa:</strong> exigir documentos oficiales, mapear oferta de juego y proteger fuentes vulnerables.</p>

          <h2>Conclusión</h2>
          <p>La ludopatía en México y en Culiacán es un fenómeno multicausal que exige políticas públicas integrales, regulación estricta, transparencia en permisos y recursos reales para prevención y tratamiento.</p>

          <p class="small">Café Expresso Portal mantiene la investigación abierta. Si tienes testimonios, documentos o datos, envíalos por el canal seguro de la redacción.</p>
        </div>

        <aside class="sidebar" aria-labelledby="sidebar-title">
          <h3 id="sidebar-title">Datos clave</h3>
          <p><strong>Prevalencia estimada:</strong> 1%–3% de la población (estudios nacionales).</p>
          <p><strong>Riesgo de suicidio:</strong> la OMS advierte aumento de riesgo hasta 15 veces en personas con ludopatía.</p>
          <div class="recuadro">
            <strong>Si te identificas</strong>
            <p class="small">Señales: priorizar apuestas; mentir sobre tiempo o dinero; pedir prestado; uso compulsivo de tarjetas; aislamiento; cambios de humor; intentos autolesivos.</p>
            <p class="small">Qué hacer: detener depósitos; conservar comprobantes; bloquear tarjetas; buscar ayuda en salud mental o grupos de apoyo; solicitar autoexclusión si está disponible.</p>
          </div>

          <h4>Preguntas enviadas</h4>
          <ul class="small">
            <li>¿Qué mecanismos de verificación de edad aplican?</li>
            <li>¿Ofrecen programas de autoexclusión?</li>
            <li>¿Qué auditorías AML han recibido?</li>
            <li>¿Qué acciones proponen para financiar atención?</li>
          </ul>

          <h4>Referencias</h4>
          <p class="small">OMS, IMSS, SciELO México, BBC Mundo, reportes locales y solicitudes de transparencia.</p>
        </aside>
      </div>
    </article>
  </main>

  <script>
    (function(){
      const images = [
        'apuestas.jpg',
        'apuestas2.jpg',
        'portada-v2.jpg',
        'imagen2.webp.png',
        'imagen3.webp.jpg',
        'imagen31.webp.jpg',
        'imagen41.webp.avif',
        'imagen5.webp.png'
      ];

      const heroImg = document.getElementById('heroImg');
      const thumbs = Array.from(document.querySelectorAll('.thumb'));
      const prevBtn = document.getElementById('prevBtn');
      const nextBtn = document.getElementById('nextBtn');
      let currentIndex = 0;

      function setHero(src, index){
        const test = new Image();
        test.onload = function(){
          heroImg.style.opacity = 0;
          setTimeout(()=> {
            heroImg.src = src;
            heroImg.alt = `Portada ${index + 1}`;
            heroImg.style.opacity = 1;
            currentIndex = index;
            highlightThumb(index);
          }, 360);
        };
        test.onerror = function(){
          console.warn('No se encontró la imagen:', src);
        };
        test.src = src;
      }

      function highlightThumb(index){
        thumbs.forEach((t, i) => {
          t.style.boxShadow = i === index ? '0 8px 20px rgba(0,0,0,0.18)' : 'none';
          t.style.border = i === index ? '2px solid var(--accent)' : '1px solid #e6e6e6';
        });
      }

      thumbs.forEach((thumb, i) => {
        thumb.addEventListener('click', () => setHero(thumb.dataset.src || thumb.src, i));
        thumb.addEventListener('keydown', (e) => {
          if(e.key === 'Enter' || e.key === ' ') {
            e.preventDefault();
            setHero(thumb.dataset.src || thumb.src, i);
          }
        });
      });

      prevBtn.addEventListener('click', () => {
        const nextIndex = (currentIndex - 1 + images.length) % images.length;
        setHero(images[nextIndex], nextIndex);
      });
      nextBtn.addEventListener('click', () => {
        const nextIndex = (currentIndex + 1) % images.length;
        setHero(images[nextIndex], nextIndex);
      });

      document.getElementById('hero').addEventListener('click', () => {
        const nextIndex = (currentIndex + 1) % images.length;
        setHero(images[nextIndex], nextIndex);
      });

      (function init(){
        let found = false;
        for(let i=0;i<images.length;i++){
          const test = new Image();
          test.onload = (function(index, src){ return function(){ if(!found){ setHero(src, index); found = true; }} })(i, images[i]);
          test.onerror = function(){ /* no hacer nada */ };
          test.src = images[i];
        }
        setTimeout(()=> {
          if(!found){
            highlightThumb(0);
          }
        }, 1200);
      })();
    })();
  </script>
</body>
</html>

