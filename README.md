<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>La Ludopatía en Culiacán — Investigación</title>

  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;400;700&family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#ffffff;
      --text:#111111;
      --muted:#6b6b6b;
      --accent:#b30000;
      --serif:"Merriweather", Georgia, "Times New Roman", serif;
      --sans:"Inter", "Helvetica Neue", Arial, sans-serif;
      --max-width:1100px;
    }
    html,body{height:100%}
    body{
      margin:0;
      font-family:var(--sans);
      color:var(--text);
      background:var(--bg);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.4;
    }
    h1,h2,h3,h4,h5,h6{margin:0 0 8px 0; line-height:1.08}
    p{margin:0 0 10px 0; color:var(--text); font-size:15.5px}
    .container{
      max-width:var(--max-width);
      margin:24px auto;
      padding:0 20px;
    }
    .masthead{
      display:flex;
      align-items:flex-end;
      gap:16px;
      border-bottom:1px solid #e6e6e6;
      padding-bottom:12px;
      margin-bottom:18px;
    }
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:72px;height:72px;background:#111;color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700;font-family:var(--serif);font-size:18px;letter-spacing:1px}
    .title{font-family:var(--serif);font-size:18px;color:var(--text)}
    .subtitle{font-size:11px;color:var(--muted);margin-top:4px}
    .meta{margin-left:auto;text-align:right;color:var(--muted);font-size:12.5px}

    .hero{display:grid;grid-template-columns:1fr 380px;gap:22px;align-items:start;margin-bottom:22px}
    .hero-main{background:#fafafa;padding:18px;border-radius:6px;box-shadow:0 6px 18px rgba(15,15,15,0.04)}
    .kicker{display:inline-block;color:var(--accent);font-weight:700;font-size:12px;text-transform:uppercase;margin-bottom:8px}
    .headline{font-family:var(--serif);font-size:30px;margin:6px 0 10px 0}
    .standfirst{color:var(--muted);font-size:15px;margin-bottom:12px}
    .byline{font-size:12.5px;color:var(--muted);margin-bottom:10px}

    .hero-image{width:100%;height:480px;background:#ddd;border-radius:6px;overflow:hidden;position:relative}
    .hero-image img{width:100%;height:100%;object-fit:cover;object-position:center 40%;display:block;transition:transform .45s ease}
    .hero-image:hover img{transform:scale(1.02)}
    .hero-caption{position:absolute;left:12px;bottom:12px;background:rgba(0,0,0,0.6);color:#fff;padding:10px 12px;font-size:13px;border-radius:4px;max-width:85%}

    .side{display:flex;flex-direction:column;gap:14px}
    .card{background:#fff;border-radius:6px;padding:12px;box-shadow:0 6px 18px rgba(15,15,15,0.03);border:1px solid #f0f0f0}
    .card h4{margin:0 0 6px 0;font-size:14px;font-family:var(--serif)}
    .card p{margin:0;color:var(--muted);font-size:13px}

    .article{display:grid;grid-template-columns:1fr 320px;gap:24px;margin-top:16px}
    .article-main{font-size:15.5px;color:var(--text)}
    .article-main h2{font-family:var(--serif);font-size:20px;margin-top:22px;margin-bottom:8px}
    .pull-quote{font-family:var(--serif);font-size:18px;color:var(--accent);border-left:4px solid var(--accent);padding:10px 14px;margin:16px 0;background:#fff8f8}

    /* Testimonios y pies */
    .testimonios{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin:14px 0 22px 0}
    .testimonio{display:flex;flex-direction:column;align-items:stretch;position:relative}
    .testimonio a{display:block;position:relative;height:160px;border-radius:6px;overflow:hidden}
    .testimonio img{width:100%;height:100%;object-fit:cover;object-position:center 40%;display:block;transition:transform .35s ease}
    .testimonio a:hover img{transform:scale(1.03)}
    .overlay{position:absolute;left:0;right:0;bottom:0;padding:12px;background:linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.65) 60%);color:#fff}
    .thumb-caption{margin-top:8px;font-size:13px;color:var(--muted);padding:0 6px;line-height:1.3}
    .hook{position:absolute;right:12px;top:12px;background:rgba(255,255,255,0.08);padding:6px 8px;border-radius:4px;font-size:12px;color:#fff;font-weight:600}

    /* Capture ayuda block */
    .capture-test{margin:0 0 18px 0;border-radius:6px;overflow:hidden;position:relative;max-width:100%}
    .capture-test img{display:block;width:100%;height:auto;object-fit:cover;object-position:center 40%}
    .capture-caption{padding:10px 12px;font-size:14px;color:var(--muted);background:transparent}
    .btn-access-test{display:inline-block;margin-top:8px;background:var(--accent);color:#fff;text-decoration:none;padding:8px 12px;border-radius:6px;font-weight:600;border:0;cursor:pointer}
    .btn-access-test:focus{outline:3px solid #ffd6d6;outline-offset:3px}

    .sidebar{position:sticky;top:24px;align-self:start;display:flex;flex-direction:column;gap:12px}
    .sidebar .box{padding:10px;border-radius:6px;background:#fff;border:1px solid #f0f0f0}
    .sidebar h5{margin:0 0 6px 0;font-family:var(--serif);font-size:14px}
    .sidebar p{margin:0;color:var(--muted);font-size:13px}
    .photo-credit{display:block;font-size:12px;color:var(--muted);margin-top:8px}
    footer{margin-top:28px;padding-top:18px;border-top:1px solid #e6e6e6;color:var(--muted);font-size:13px}
    :focus{outline:3px solid #ffd6d6;outline-offset:3px}

    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .hero-image{height:320px}
      .article{grid-template-columns:1fr}
      .testimonios{grid-template-columns:1fr}
      .container{padding:0 16px}
    }

    /* ===== Modal del cuestionario ===== */
    .quiz-modal{position:fixed;inset:0;display:flex;align-items:center;justify-content:center;z-index:1200}
    .quiz-backdrop{position:absolute;inset:0;background:rgba(0,0,0,0.55)}
    .quiz-panel{position:relative;width:min(880px,94%);max-height:90vh;overflow:auto;background:#fff;border-radius:8px;box-shadow:0 20px 60px rgba(0,0,0,0.35);z-index:2}
    .quiz-header{display:flex;align-items:center;justify-content:space-between;padding:16px 20px;border-bottom:1px solid #eee}
    .quiz-header h3{margin:0;font-family:var(--serif);font-size:18px}
    .quiz-close{background:transparent;border:0;font-size:26px;line-height:1;cursor:pointer;color:#333}
    .quiz-body{padding:18px 20px;font-size:15px;color:var(--text)}
    .quiz-intro{margin:0 0 12px 0;color:var(--muted)}
    .quiz-list{list-style:none;padding:0;margin:0 0 12px 0}
    .quiz-list li{margin-bottom:12px;padding:10px;border-radius:6px;background:#fafafa;display:flex;align-items:center;gap:12px}
    .quiz-question{flex:1;font-family:var(--sans);font-size:15px}
    .quiz-options{display:flex;gap:10px}
    .quiz-options label{display:inline-flex;align-items:center;gap:6px;cursor:pointer;padding:6px 10px;border-radius:6px;background:#fff;border:1px solid #e6e6e6}
    .quiz-actions{display:flex;gap:10px;margin-top:12px}
    .btn-primary{background:var(--accent);color:#fff;border:0;padding:8px 12px;border-radius:6px;cursor:pointer}
    .btn-secondary{background:#f3f3f3;color:#333;border:0;padding:8px 12px;border-radius:6px;cursor:pointer}
    .btn-link{background:transparent;border:0;color:var(--accent);padding:12px;cursor:pointer}
    .quiz-result{margin-top:14px;padding:12px;border-radius:6px;background:#fff8f8;border-left:4px solid var(--accent)}
    .quiz-footer{padding:12px 20px;border-top:1px solid #eee;text-align:right}
    @media (max-width:700px){ .quiz-panel{width:96%} .quiz-list li{flex-direction:column;align-items:flex-start} }
  </style>
</head>
<body>
  <div class="container">
    <!-- Masthead -->
    <header class="masthead" role="banner">
      <div class="brand" aria-hidden="true">
        <div class="logo">AP</div>
        <div>
          <div class="title">Apuestas</div>
          <div class="subtitle">Investigación especial — Culiacán</div>
        </div>
      </div>

      <div class="meta">
        <div><strong>Miguel A. Miranda Félix</strong></div>
        <div>Enero 2026 — Facultad de Filosofía y Letras, UAS</div>
      </div>
    </header>

    <!-- Hero -->
    <section class="hero" aria-labelledby="main-headline">
      <article class="hero-main">
        <div class="kicker">Investigación</div>
        <h1 id="main-headline" class="headline">La ludopatía en Culiacán: una adicción silenciosa que devora vidas y dinero</h1>
        <p class="standfirst">Entre maquinitas en colonias populares, plataformas digitales y casinos con permisos ambiguos, la adicción al juego se ha convertido en un problema de salud pública y seguridad financiera. Este reportaje cruza testimonios, datos institucionales y documentos en trámite para mostrar la magnitud del daño.</p>

        <div class="byline">Por <strong>Miguel Alfredo Miranda Félix</strong> — Investigación y reportaje</div>

        <p style="color:var(--muted);font-size:13.5px;margin-top:6px;">
          Resumen: Este reportaje documenta factores de riesgo, trayectorias clínicas, impacto económico y vínculos con lavado de dinero en Sinaloa. Incluye testimonios, solicitudes de información y propuestas de política pública.
        </p>
      </article>

      <aside class="side" aria-label="Portada y destacados">
        <figure class="hero-image" role="img" aria-label="Portada principal">
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas.jpg" alt="Portada: Mano contando billetes; fondo nocturno con letreros de apuestas y silueta de espaldas" loading="lazy" width="1200" height="800">
          <figcaption class="hero-caption">Portada: Maquinitas y minicasinos en colonias populares; la accesibilidad alimenta la adicción.</figcaption>
        </figure>

        <div class="card">
          <h4>Hallazgos clave</h4>
          <p>La investigación identifica: normalización del juego entre jóvenes; vacíos regulatorios; 13 casinos vinculados a operaciones sospechosas; y testimonios de prostitución y delitos para financiar apuestas.</p>
        </div>

        <div class="card">
          <h4>Cómo ayudar</h4>
          <p>Se proponen campañas de prevención, regulación estricta de plataformas digitales, programas de rehabilitación accesibles y transparencia en licencias.</p>
        </div>
      </aside>
    </section>

    <!-- Bloque: imagen de ayuda + enlace para abrir el cuestionario -->
    <section aria-label="Captura principal">
      <figure class="capture-test" aria-labelledby="captureTitle">
        <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/ayuda.jpg" alt="Cómo ayudar: campañas de prevención, regulación y programas de rehabilitación" loading="lazy" width="1200" height="800">
        <figcaption id="captureTitle" class="capture-caption">
          <strong>Cómo ayudar</strong><br>
          Se proponen campañas de prevención, regulación estricta de plataformas digitales, programas de rehabilitación accesibles y transparencia en licencias.
          <br>
          <a href="#quizModal" class="btn-access-test" role="button" aria-haspopup="dialog" aria-controls="quizModal">Acceder al test</a>
        </figcaption>
      </figure>
    </section>

    <!-- Article body -->
    <main class="article" role="main">
      <section class="article-main">
        <h2>Contexto: de entretenimiento a dependencia</h2>
        <p>La ludopatía, o trastorno por juego, es una adicción sin sustancia que afecta a miles de personas en México. En Culiacán, la proliferación de casinos, minicasinos y plataformas digitales ha facilitado el acceso al juego, especialmente entre adolescentes y jóvenes universitarios.</p>

        <div class="pull-quote">“La ludopatía es un asesino silencioso que te lleva a la cárcel, a la locura o a la muerte.” — Testimonio recogido en Culiacán</div>

        <h2 id="testimonios">Testimonios que atrapan</h2>

        <div class="testimonios" aria-label="Testimonios destacados">
          <figure class="testimonio" role="article" aria-labelledby="t1">
            <a href="#detalle-impacto-social" title="Abrir testimonio: Impacto social" aria-controls="detalle-impacto-social">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas_supervivencia.jpg" loading="lazy" alt="Manos intercambiando un sobre con billetes; fondo nocturno con letreros de apuestas" width="1200" height="800">
              <div class="overlay">
                <div class="quote">“Apostadores llegan hasta a prostituirse.”</div>
                <div class="credit">Publicación local; relato de supervivencia económica</div>
              </div>
            </a>
            <figcaption class="thumb-caption">
              <strong>Impacto social:</strong> relatos de supervivencia que muestran la marginalización económica.
              <button class="quiz-open" data-quiz="screening" aria-haspopup="dialog" aria-controls="quizModal">¿Me afecta?</button>
            </figcaption>
            <div class="hook">Impacto social</div>
          </figure>

          <figure class="testimonio" role="article" aria-labelledby="t2">
            <a href="#detalle-toque-humano" title="Abrir testimonio: Toque humano" aria-controls="detalle-toque-humano">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino_mentira_espejo.jpg" loading="lazy" alt="Mesa con fichas y billetes; espejo agrietado que refleja luces de neón" width="1200" height="800">
              <div class="overlay">
                <div class="quote">“El casino es una mentira: no se hizo para perder, sino para que los dueños ganen.”</div>
                <div class="credit">Caso clínico; Los Mochis</div>
              </div>
            </a>
            <figcaption class="thumb-caption">
              <strong>Toque humano:</strong> testimonio clínico que muestra la progresión del trastorno.
              <button class="quiz-open" data-quiz="screening" aria-haspopup="dialog" aria-controls="quizModal">¿Me afecta?</button>
            </figcaption>
            <div class="hook">Toque humano</div>
          </figure>

          <figure class="testimonio" role="article" aria-labelledby="t3">
            <a href="#detalle-perdida-economica" title="Abrir testimonio: Pérdida económica" aria-controls="detalle-perdida-economica">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/perdida_economica_caja.jpg" loading="lazy" alt="Caja de mudanza abierta frente a una puerta cerrada; objetos personales dispersos" width="1200" height="800">
              <div class="overlay">
                <div class="quote">“He perdido fácil más de dos millones de pesos.”</div>
                <div class="credit">Testimonio personal; recuperación parcial</div>
              </div>
            </a>
            <figcaption class="thumb-caption">
              <strong>Pérdida económica:</strong> el rastro tangible del endeudamiento y la venta de bienes.
              <button class="quiz-open" data-quiz="screening" aria-haspopup="dialog" aria-controls="quizModal">¿Me afecta?</button>
            </figcaption>
            <div class="hook">Pérdida económica</div>
          </figure>
        </div>

        <!-- Secciones ampliadas -->
        <h2 id="detalle-impacto-social">Impacto social — Testimonio ampliado</h2>
        <p>Relato ampliado: en comunidades con precariedad económica, la presión por obtener recursos rápidos empuja a algunas personas a medidas extremas. Este testimonio documenta cómo la deuda y la estigmatización empujan a la marginalidad y a prácticas de supervivencia que dañan a familias enteras.</p>

        <h2 id="detalle-toque-humano">Toque humano — Caso clínico (Los Mochis)</h2>
        <p>Relato clínico: la progresión desde el juego recreativo hasta el trastorno por juego puede incluir convulsiones por estrés, intentos autolesivos y pérdida de empleo. Este caso muestra la necesidad de protocolos de derivación entre servicios de salud y redes comunitarias.</p>

        <h2 id="detalle-perdida-economica">Pérdida económica — Testimonio ampliado</h2>
        <p>Relato económico: la pérdida de patrimonio y el endeudamiento masivo son consecuencias frecuentes. En este testimonio, la persona describe el uso de tarjetas, préstamos y la venta de bienes para sostener la conducta adictiva, así como el proceso de recuperación parcial.</p>

        <h2>Consecuencias sociales y económicas</h2>
        <p>Las consecuencias son devastadoras: desintegración familiar, endeudamiento, pérdida de patrimonio, delitos para financiar apuestas y riesgos para la salud mental, incluyendo ansiedad, depresión y riesgo de suicidio.</p>

        <h2>Vínculos con lavado de dinero y complicidad institucional</h2>
        <p>La Unidad de Inteligencia Financiera ha detectado operaciones sospechosas en casinos y plataformas. En Sinaloa, inspecciones y reportes periodísticos señalan la posible utilización de establecimientos de juego como fachadas para blanquear capitales.</p>

        <h2>Recomendaciones y propuestas</h2>
        <ul>
          <li>Campañas de prevención dirigidas a adolescentes y universitarios.</li>
          <li>Regulación estricta de casinos y plataformas digitales, con auditorías públicas y controles AML.</li>
          <li>Programas de rehabilitación accesibles y gratuitos, con protocolos de derivación entre salud y servicios sociales.</li>
          <li>Transparencia en el otorgamiento de licencias y sanciones claras para operadores irregulares.</li>
        </ul>

        <p style="margin-top:18px;color:var(--muted);font-size:14px;"><strong>Nota del autor:</strong> Las identidades de las personas afectadas han sido protegidas. Las cifras y hallazgos se basan en fuentes locales, institucionales y testimonios periodísticos; se recomienda la verificación documental para uso académico o judicial.</p>
      </section>

      <!-- Sidebar -->
      <aside class="sidebar" aria-label="Información complementaria">
        <div class="box">
          <h5>Documentos solicitados</h5>
          <p>Carpetas de investigación, actas de aseguramiento, cifras de atención por trastorno del juego (2021–2024) y borrador de reforma a la Ley de Juegos y Sorteos.</p>
        </div>

        <div class="box">
          <h5>Guía rápida: señales</h5>
          <p>Priorizar apuestas; mentir sobre tiempo o dinero; pedir prestado para apostar; uso compulsivo de tarjetas; aislamiento; cambios de humor extremos.</p>
        </div>

        <div class="box">
          <h5>Recuadro práctico</h5>
          <p>Si te identificas: detener depósitos, conservar comprobantes, bloquear tarjetas, hablar con un familiar y buscar atención en salud mental o grupos de apoyo.</p>
        </div>

        <div class="box">
          <h5>Referencias seleccionadas</h5>
          <p style="color:var(--muted);font-size:13px;margin-top:6px;">
            CIJ; UAS; Condusef; UIF; Ríodoce; El Sol de Sinaloa; El Debate; El Siglo de Torreón.
          </p>
        </div>
      </aside>
    </main>

    <!-- Footer -->
    <footer role="contentinfo">
      <div style="display:flex;gap:18px;flex-wrap:wrap;align-items:center;justify-content:space-between">
        <div>
          <strong>Apuestas — Investigación</strong><br>
          Facultad de Filosofía y Letras, Universidad Autónoma de Sinaloa — Enero 2026
        </div>

        <div style="text-align:right;color:var(--muted);font-size:13px;">
          <div>Edición y reportaje: Miguel Alfredo Miranda Félix</div>
          <div>Contacto: correo de redacción — pendiente de confirmación</div>
        </div>
      </div>
    </footer>
  </div>

  <!-- ===== Modal del cuestionario (si no está ya incluido) ===== -->
  <div id="quizModal" class="quiz-modal" role="dialog" aria-modal="true" aria-labelledby="quizTitle" hidden>
    <div class="quiz-backdrop" data-close="true" tabindex="-1"></div>
    <div class="quiz-panel" role="document">
      <header class="quiz-header">
        <h3 id="quizTitle">Autoevaluación rápida: ¿estoy afectado por el juego?</h3>
        <button class="quiz-close" aria-label="Cerrar cuestionario">&times;</button>
      </header>

      <main class="quiz-body" id="quizContent">
        <p class="quiz-intro">Responde con sinceridad. Este cuestionario es orientativo y no sustituye una evaluación profesional.</p>

        <form id="quizForm" aria-describedby="quizHelp">
          <ol class="quiz-list" id="quizQuestions" role="list"></ol>

          <div class="quiz-actions">
            <button type="button" id="quizSubmit" class="btn-primary">Ver resultado</button>
            <button type="button" id="quizReset" class="btn-secondary">Reiniciar</button>
          </div>
        </form>

        <div id="quizResult" class="quiz-result" hidden aria-live="polite"></div>

        <p id="quizHelp" class="quiz-help">Si el resultado indica riesgo, considera hablar con un profesional de salud mental o con servicios de apoyo locales.</p>
      </main>

      <footer class="quiz-footer">
        <button class="btn-link" id="quizCloseFooter">Volver al artículo</button>
      </footer>
    </div>
  </div>

  <!-- ===== Scripts: prefetch, smooth scroll, modal y cuestionario ===== -->
  <script>
  (function(){
    // Fallback SVG for broken images
    const fallback = "data:image/svg+xml;charset=UTF-8," + encodeURIComponent(
      '<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="800"><rect width="100%" height="100%" fill="#e9e9e9"/><text x="50%" y="50%" font-family="Arial, sans-serif" font-size="20" fill="#777" text-anchor="middle">Imagen pendiente</text></svg>'
    );
    document.querySelectorAll('img').forEach(img=>{
      img.addEventListener('error', function(){ if(this.src !== fallback) this.src = fallback; });
    });

    // Prefetch imagen al pasar el cursor sobre testimonios
    document.querySelectorAll('.testimonio a').forEach(link=>{
      link.addEventListener('mouseenter', function(){
        const img = this.querySelector('img');
        if(img && !img.dataset.prefetched){
          const pre = new Image();
          pre.src = img.src;
          img.dataset.prefetched = '1';
        }
      });
    });

    // Smooth scroll + foco accesible para anclas internas
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', function(e){
        const href = this.getAttribute('href');
        if(href === '#quizModal'){ /* handled by modal opener below */ return; }
        const targetId = href.slice(1);
        const target = document.getElementById(targetId);
        if(target){
          e.preventDefault();
          target.scrollIntoView({behavior:'smooth', block:'start'});
          target.setAttribute('tabindex','-1');
          target.focus({preventScroll:true});
        }
      });
    });

    // ===== Modal open/close from capture button and quiz-open buttons =====
    const modal = document.getElementById('quizModal');
    const openFromCapture = document.querySelector('.btn-access-test');
    const openButtons = document.querySelectorAll('.quiz-open');
    const closeButtons = modal ? modal.querySelectorAll('.quiz-close, #quizCloseFooter, .quiz-backdrop') : [];

    function openModal(){
      if(!modal) return;
      modal.hidden = false;
      document.body.style.overflow = 'hidden';
      // focus first radio after questions render
      setTimeout(()=> {
        const first = modal.querySelector('input[type="radio"]');
        if(first) first.focus();
        else modal.querySelector('.quiz-close')?.focus();
      }, 120);
    }
    function closeModal(){
      if(!modal) return;
      modal.hidden = true;
      document.body.style.overflow = '';
      // return focus to last trigger if possible
      const last = document.querySelector('.btn-access-test, .quiz-open');
      if(last) last.focus();
    }

    openFromCapture?.addEventListener('click', function(e){ e.preventDefault(); openModal(); });
    openButtons.forEach(btn => btn.addEventListener('click', function(e){ e.preventDefault(); openModal(); }));

    closeButtons.forEach(el=>{
      el.addEventListener('click', function(e){
        closeModal();
      });
    });

    document.addEventListener('keydown', function(e){
      if(e.key === 'Escape' && modal && !modal.hidden) closeModal();
    });

    // ===== Cuestionario: preguntas, render y evaluación =====
    const questions = [
      "¿Sientes que apuestas más tiempo o dinero del que planeabas?",
      "¿Has intentado reducir o dejar de jugar sin éxito?",
      "¿Mientes a familiares o amigos sobre cuánto juegas o pierdes?",
      "¿Has pedido prestado dinero o vendido bienes para apostar?",
      "¿El juego ha afectado tu trabajo, estudios o relaciones?",
      "¿Te sientes inquieto o irritable cuando intentas dejar de jugar?",
      "¿Usas el juego como escape de problemas o emociones negativas?",
      "¿Has vuelto a jugar para recuperar pérdidas anteriores?"
    ];
    const thresholds = { low: 0, moderate: 3, high: 5 };

    const quizList = document.getElementById('quizQuestions');
    const quizSubmit = document.getElementById('quizSubmit');
    const quizReset = document.getElementById('quizReset');
    const quizResult = document.getElementById('quizResult');
    const quizForm = document.getElementById('quizForm');

    function renderQuestions(){
      if(!quizList) return;
      quizList.innerHTML = '';
      questions.forEach((q, i) => {
        const li = document.createElement('li');
        li.innerHTML = `
          <div class="quiz-question" id="q${i+1}">${i+1}. ${q}</div>
          <div class="quiz-options" role="radiogroup" aria-labelledby="q${i+1}">
            <label><input type="radio" name="q${i}" value="1"> Sí</label>
            <label><input type="radio" name="q${i}" value="0" checked> No</label>
          </div>
        `;
        quizList.appendChild(li);
      });
    }

    function evaluate(){
      if(!quizForm) return;
      const formData = new FormData(quizForm);
      let score = 0;
      for(let i=0;i<questions.length;i++){
        const val = formData.get('q'+i);
        score += val ? Number(val) : 0;
      }
      let message = '';
      if(score >= thresholds.high){
        message = `<strong>Riesgo alto</strong>. Tu respuesta sugiere que el juego está teniendo un impacto significativo. Considera buscar ayuda profesional y apoyo inmediato.`;
      } else if(score >= thresholds.moderate){
        message = `<strong>Riesgo moderado</strong>. Hay señales de problema: habla con un profesional, un familiar de confianza o un grupo de apoyo.`;
      } else {
        message = `<strong>Bajo riesgo</strong>. No obstante, si te preocupa tu relación con el juego, vigila las señales y busca orientación si cambian.`;
      }

      quizResult.innerHTML = `
        <div><strong>Puntaje:</strong> ${score} de ${questions.length}</div>
        <div style="margin-top:8px">${message}</div>
        <div style="margin-top:10px;font-size:13px;color:var(--muted)">
          Este cuestionario es orientativo y no reemplaza una evaluación clínica. Si estás en riesgo o en crisis, contacta servicios de salud mental o líneas de ayuda locales.
        </div>
        <div style="margin-top:10px">
          <button id="quizResources" class="btn-secondary">Ver recursos y pasos recomendados</button>
        </div>
      `;
      quizResult.hidden = false;

      const resBtn = document.getElementById('quizResources');
      resBtn?.addEventListener('click', function(){
        quizResult.insertAdjacentHTML('beforeend', `
          <div style="margin-top:12px;padding:10px;border-radius:6px;background:#fff;">
            <strong>Pasos recomendados</strong>
            <ul style="margin:8px 0 0 18px;color:var(--muted)">
              <li>Habla con alguien de confianza sobre lo que estás viviendo.</li>
              <li>Contacta a un profesional de salud mental o a servicios de adicciones.</li>
              <li>Bloquea o limita accesos a plataformas de apuestas y tarjetas.</li>
              <li>Conserva comprobantes y evita decisiones financieras impulsivas.</li>
            </ul>
          </div>
        `);
        resBtn.disabled = true;
      });
    }

    quizSubmit?.addEventListener('click', function(){ evaluate(); });
    quizReset?.addEventListener('click', function(){ renderQuestions(); quizResult.hidden = true; });

    // Inicializar preguntas
    renderQuestions();
  })();
  </script>
</body>
</html>


