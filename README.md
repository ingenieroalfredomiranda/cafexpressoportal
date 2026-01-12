<!DOCTYPE html>
<html lang="es-MX">
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />

    <!-- Jekyll SEO / Open Graph -->
    <title>cafexpressoportal | sitio de noticias de investigación de la carrera de periodismo UAS (Alfredo Miranda)</title>
    <meta name="generator" content="Jekyll v3.10.0" />
    <meta name="description" content="sitio de noticias de investigación de la carrera de periodismo UAS (Alfredo Miranda)" />
    <meta name="keywords" content="periodismo, investigación, UAS, noticias, cafexpressoportal, Alfredo Miranda" />

    <!-- Open Graph -->
    <meta property="og:title" content="cafexpressoportal" />
    <meta property="og:locale" content="es_MX" />
    <meta property="og:description" content="sitio de noticias de investigación de la carrera de periodismo UAS (Alfredo Miranda)" />
    <meta property="og:url" content="https://ingenieroalfredomiranda.github.io/cafexpressoportal/" />
    <meta property="og:site_name" content="cafexpressoportal" />
    <meta property="og:type" content="website" />
    <meta property="og:image" content="https://ingenieroalfredomiranda.github.io/cafexpressoportal/assets/cafe.png" />

    <!-- Twitter -->
    <meta name="twitter:card" content="summary_large_image" />
    <meta property="twitter:title" content="cafexpressoportal" />
    <meta name="twitter:image" content="https://ingenieroalfredomiranda.github.io/cafexpressoportal/assets/cafe.png" />

    <!-- Canonical -->
    <link rel="canonical" href="https://ingenieroalfredomiranda.github.io/cafexpressoportal/" />

    <!-- Structured Data -->
    <script type="application/ld+json">
      {
        "@context":"https://schema.org",
        "@type":"WebSite",
        "description":"sitio de noticias de investigación de la carrera de periodismo UAS (Alfredo Miranda)",
        "headline":"cafexpressoportal",
        "name":"cafexpressoportal",
        "url":"https://ingenieroalfredomiranda.github.io/cafexpressoportal/",
        "image":"https://ingenieroalfredomiranda.github.io/cafexpressoportal/assets/cafe.png"
      }
    </script>

    <!-- Styles -->
    <link rel="stylesheet" href="/cafexpressoportal/assets/css/style.css?v=51ab0bafa6680ed18ba8703b2a05c6a3514c81b2" />

    <!-- Estilos locales (temporal). Extrae esto a style.css en producción -->
    <style>
      :root {
        --accent: #ff5252;
        --muted: #6b6b6b;
        --caption-bg: rgba(0,0,0,0.75);
      }
    </style>
  </head>

      }

      /* Contenedor */
      .container-lg { max-width: 980px; margin: 0 auto; padding: 0 16px; }

      /* Imágenes */
      .imagen-ajustada,
      .responsive-img {
        width: 100%;
        height: auto;
        display: block;
        object-fit: cover;
        border-radius: 6px;
        max-width: 100%;
      }

      /* Figuras y overlays */
      .hero-image,
      .info-image,
      .capture-test,
      .testimonio {
        position: relative;
        margin: 0 0 24px 0;
      }

      .hero-caption {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        background: var(--caption-bg);
        color: #fff;
        padding: 16px;
        border-radius: 0 0 6px 6px;
      }

      .hero-caption.text-left { text-align: left; padding: 20px; background: rgba(0,0,0,0.75); }
      .hero-caption.text-center { text-align: center; padding: 16px; background: rgba(0,0,0,0.7); }

      /* Tipografías responsivas */
      .hero-title { font-size: clamp(18px, 4vw, 22px); font-weight: 700; color: var(--accent); margin-bottom: 8px; text-shadow: 0 1px 2px rgba(0,0,0,0.6); }
      .hero-heading { font-size: clamp(20px, 4vw, 26px); font-weight: 700; color: var(--accent); margin: 0; text-shadow: 0 1px 2px rgba(0,0,0,0.6); }
      .hero-subheading { font-size: clamp(16px, 3vw, 18px); font-weight: 400; color: #f0f0f0; margin: 4px 0 12px 0; }
      .hero-text { font-size: 14px; line-height: 1.5; margin: 0 0 8px 0; color: #fff; }
      .hero-credit { font-size: 12px; color: #ccc; margin-top: 10px; }

      /* Info caption (no overlay) */
      .info-caption { position: static; background: transparent; color: #444; padding-top: 10px; text-align: center; font-size: 14px; }
      .info-caption h4 { margin: 0 0 8px 0; font-size: 16px; color: #222; }

      .shadowed { box-shadow: 0 2px 8px rgba(0,0,0,0.25); }

      /* Botones */
      .btn-access-test {
        background: var(--accent);
        color: #fff;
        border: none;
        padding: 10px 18px;
        border-radius: 4px;
        cursor: pointer;
        font-size: 14px;
        display: inline-block;
        margin-top: 12px;
      }

      .btn-access-test:hover,
      .btn-access-test:focus { background: #e04848; outline: none; }

      .kicker { font-size: 13px; color: var(--muted); margin-bottom: 6px; }
      .headline { font-size: clamp(20px, 3.5vw, 28px); margin: 6px 0 12px 0; }
      .byline { font-size: 14px; color: #333; margin-bottom: 8px; }
      .summary { color: var(--muted); font-size: 13.5px; margin-top: 6px; }

      .testimonio img { object-fit: contain; }
      .testimonio figcaption {
        background: rgba(0,0,0,0.75);
        color: #fff;
        padding: 16px;
        border-radius: 0 0 6px 6px;
        text-align: center;
      }

      /* Modal basic styles (minimal) */
      .quiz-modal { position: fixed; inset: 0; display: grid; place-items: center; z-index: 1200; }
      .quiz-modal[hidden] { display: none; }
      .quiz-backdrop { position: absolute; inset: 0; background: rgba(0,0,0,0.5); }
      .quiz-panel { position: relative; background: #fff; color: #111; width: min(720px, 96%); max-height: 90vh; overflow: auto; border-radius: 8px; box-shadow: 0 8px 32px rgba(0,0,0,0.25); padding: 0; }
      .quiz-header { display:flex; align-items:center; justify-content:space-between; padding: 16px; border-bottom: 1px solid #eee; }
      .quiz-body { padding: 16px; }
      .quiz-actions { display:flex; gap:12px; margin-top:12px; }
      .btn-primary { background: #0b5fff; color:#fff; border:none; padding:8px 14px; border-radius:4px; cursor:pointer; }
      .btn-secondary { background:#f0f0f0; color:#111; border:none; padding:8px 14px; border-radius:4px; cursor:pointer; }

      @media (max-width: 480px) {
        .hero-caption { padding: 12px; }
        .btn-access-test { padding: 8px 14px; font-size: 13px; }
        .quiz-panel { width: 96%; }
      }
    </style>
  </head>

  <body>
    <main class="container-lg px-3 my-5 markdown-body" role="main">
      <h1><a href="https://ingenieroalfredomiranda.github.io/cafexpressoportal/">cafexpressoportal</a></h1>

      <!-- Hero -->
      <section class="hero" aria-labelledby="main-headline">
        <article class="hero-main">
          <div class="kicker">Investigación</div>
          <h1 id="main-headline" class="headline">
            La ludopatía en Culiacán: una adicción silenciosa que devora vidas y dinero
          </h1>

          <div class="byline">
            Por <strong>Cafe Expreso Portal</strong> — Investigación y reportaje
          </div>

          <p class="summary">
            Resumen: Este reportaje documenta factores de riesgo, trayectorias clínicas, impacto económico y vínculos con lavado de dinero en Sinaloa. Incluye testimonios, solicitudes de información y propuestas de política pública.
          </p>

          <!-- Portada principal -->
          <figure class="hero-image">
            <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas.jpg"
                 alt="Portada principal: apuestas en Culiacán"
                 class="imagen-ajustada responsive-img"
                 loading="lazy" />
            <figcaption class="hero-caption text-center" role="note">
              <div class="hero-title">Apuestas en Culiacán</div>
            </figcaption>
          </figure>
        </article>
      </section>

      <!-- Captura principal -->
      <section aria-label="Captura principal">
        <figure class="capture-test" aria-labelledby="captureTitle">
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/ayuda.jpg"
               alt="Cómo ayudar: campañas de prevención, regulación y programas de rehabilitación"
               loading="lazy"
               class="imagen-ajustada responsive-img" />
          <figcaption id="captureTitle" class="info-caption" role="note">
            <h4>Cómo ayudar</h4>
            Se proponen campañas de prevención, regulación estricta de plataformas digitales, programas de rehabilitación accesibles y transparencia en licencias.
            <br />
            <button id="openQuiz" type="button" class="btn-access-test" aria-haspopup="dialog" aria-controls="quizModal" aria-label="Abrir test sobre ludopatía">Acceder al test</button>
          </figcaption>
        </figure>
      </section>

      <!-- Cartel informativo -->
      <figure class="info-image">
        <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/ludopatia-cartel.jpg"
             alt="Cartel sobre juego patológico: síntomas, ayuda psicológica 24 horas y contacto de emergencia"
             class="imagen-ajustada responsive-img shadowed"
             loading="lazy" />
        <figcaption class="info-caption" role="note">
          <h4>JUEGO PATOLÓGICO — LUDOPATÍA</h4>
          <p>Señales de adicción al juego: pensamiento persistente, necesidad de apostar más, irritabilidad, mentiras, pérdidas económicas y familiares.</p>
          <p><em>Si te identificas, puedes necesitar ayuda. Atención psicológica 24 horas: <strong>911</strong></em></p>
          <p class="source">Fuente: Secretaría de Salud, Gobierno de Sonora.</p>
          <p><button id="openSurvey" type="button" class="btn-access-test" aria-haspopup="dialog" aria-controls="surveyModal" aria-label="Abrir encuesta sobre ludopatía">Acceder a la encuesta</button></p>
        </figcaption>
      </figure>

      <!-- Testimonios -->
      <div class="testimonios" aria-label="Testimonios destacados">
        <figure class="testimonio" role="article" aria-labelledby="t1">
          <a href="#detalle-impacto-social" title="Abrir testimonio: Impacto social">
            <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas_supervivencia.jpg"
                 loading="lazy"
                 alt="Manos intercambiando un sobre con billetes; fondo nocturno con letreros de apuestas"
                 class="imagen-ajustada responsive-img" />
          </a>
          <figcaption>
            <h5 id="t1" class="testimonial-title">Apostadores llegan hasta a prostituirse</h5>
            <p style="font-size:16px;font-style:italic;margin-bottom:12px;">Las graves conductas de la ludopatía</p>
            <a href="segunda-parte.html" class="btn-link">Haz click para seguir leyendo »</a>
          </figcaption>
        </figure>

        <figure class="testimonio" role="article" aria-labelledby="t2">
          <a href="#detalle-toque-humano" title="Abrir testimonio: Toque humano">
            <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino_mentira_espejo.jpg"
                 loading="lazy"
                 alt="Mesa con fichas y billetes; espejo agrietado que refleja luces de neón"
                 class="imagen-ajustada responsive-img" />
          </a>
          <figcaption>
            <h5 id="t2" class="testimonial-title">"Puse en riesgo hasta mi vida por la adicción al casino"</h5>
            <a href="segunda-parte.html" class="btn-link">Haz click para seguir leyendo »</a>
          </figcaption>
        </figure>

        <figure class="testimonio" role="article" aria-labelledby="t3">
          <a href="detalle.html" title="Abrir testimonio: Pérdida económica">
            <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/perdida_economica.jpg"
                 loading="lazy"
                 alt="Persona revisando cuentas y facturas; expresión de preocupación"
                 class="imagen-ajustada responsive-img" />
          </a>
          <figcaption>
            <h5 id="t3" class="testimonial-title">Pérdidas que destruyen familias</h5>
            <p style="font-size:16px;font-style:italic;margin-bottom:12px;">Historias de endeudamiento y desarraigo</p>
            <a href="segunda-parte.html" class="btn-link">Haz click para seguir leyendo »</a>
          </figcaption>
        </figure>
      </div>

      <!-- Secciones ampliadas -->
      <section id="secciones-ampliadas">
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
      </section>

      <section id="recomendaciones">
        <h2>Recomendaciones y propuestas</h2>
        <ul>
          <li>Campañas de prevención dirigidas a adolescentes y universitarios.</li>
          <li>Regulación estricta de casinos y plataformas digitales, con auditorías públicas y controles AML.</li>
          <li>Programas de rehabilitación accesibles y gratuitos, con protocolos de derivación entre salud y servicios sociales.</li>
          <li>Transparencia en el otorgamiento de licencias y sanciones claras para operadores irregulares.</li>
        </ul>

        <p style="margin-top:18px;color:var(--muted);font-size:14px;">
          <strong>Nota del autor:</strong> Las identidades de las personas afectadas han sido protegidas. Las cifras y hallazgos se basan en fuentes locales, institucionales y testimonios periodísticos; se recomienda la verificación documental para uso académico o judicial.
        </p>
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
    <footer role="contentinfo" style="padding:18px 16px;border-top:1px solid #eee;">
      <div style="display:flex;gap:18px;flex-wrap:wrap;align-items:center;justify-content:space-between">
        <div>
          <strong>Apuestas — Investigación</strong><br />
          Facultad de Filosofía y Letras, Universidad Autónoma de Sinaloa — Enero 2026
        </div>

        <div style="text-align:right;color:var(--muted);font-size:13px;">
          <div>Edición y reportaje: Miguel Alfredo Miranda Félix</div>
          <div>Contacto: correo de redacción — pendiente de confirmación</div>
        </div>
      </div>
    </footer>

    <!-- ===== Modal del cuestionario ===== -->
    <div id="quizModal" class="quiz-modal" role="dialog" aria-modal="true" aria-labelledby="quizTitle" hidden aria-hidden="true">
      <div class="quiz-backdrop" data-close="true" tabindex="-1" aria-hidden="true"></div>
      <div class="quiz-panel" role="document" aria-describedby="quizHelp">
        <header class="quiz-header">
          <h3 id="quizTitle">Autoevaluación rápida: ¿estoy afectado por el juego?</h3>
          <button class="quiz-close" aria-label="Cerrar cuestionario" type="button">&times;</button>
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

          <div id="quizResult" class="quiz-result" hidden aria-live="polite" tabindex="-1"></div>

          <p id="quizHelp" class="quiz-help">Si el resultado indica riesgo, considera hablar con un profesional de salud mental o con servicios de apoyo locales.</p>
        </main>

        <footer class="quiz-footer" style="padding:12px;border-top:1px solid #eee;text-align:right;">
          <button class="btn-link" id="quizCloseFooter" type="button">Volver al artículo</button>
        </footer>
      </div>
    </div>

    <!-- ===== Scripts ===== -->
    <script>
    (function(){
      // Smooth scroll accesible (ignora enlaces que abren el modal)
      document.querySelectorAll('a[href^="#"]').forEach(a=>{
        a.addEventListener('click', function(e){
          const href = this.getAttribute('href');
          if(!href || href === '#' || href === '#quizModal') return;
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

      // Modal open/close
      const modal = document.getElementById('quizModal');
      const openButtons = Array.from(document.querySelectorAll('.btn-access-test'));
      const closeButtons = modal ? Array.from(modal.querySelectorAll('.quiz-close, #quizCloseFooter, .quiz-backdrop')) : [];

      function setModalHidden(hidden){
        if(!modal) return;
        modal.hidden = hidden;
        modal.setAttribute('aria-hidden', hidden ? 'true' : 'false');
        const backdrop = modal.querySelector('.quiz-backdrop');
        if(backdrop) backdrop.setAttribute('aria-hidden', hidden ? 'true' : 'false');
        document.body.style.overflow = hidden ? '' : 'hidden';
      }

      function openModal(opener){
        if(!modal) return;
        modal._opener = opener || null;
        setModalHidden(false);
        setTimeout(()=> {
          const first = modal.querySelector('input[type="radio"], button, [tabindex]:not([tabindex="-1"])');
          if(first) first.focus();
          else modal.querySelector('.quiz-close')?.focus();
        }, 120);
      }

      function closeModal(){
        if(!modal) return;
        setModalHidden(true);
        const opener = modal._opener || openButtons[0];
        opener?.focus();
      }

      if(openButtons.length && modal){
        openButtons.forEach(btn => {
          btn.addEventListener('click', function(e){
            e.preventDefault();
            openModal(btn);
          });
        });
      }

      if(closeButtons.length && modal){
        closeButtons.forEach(el => {
          el.addEventListener('click', function(e){
            if(el.classList && el.classList.contains('quiz-backdrop') && el.getAttribute('data-close') !== 'true') return;
            closeModal();
          });
        });
      }

      document.addEventListener('keydown', function(e){
        if(e.key === 'Escape' && modal && !modal.hidden) closeModal();
      });

      // Evitar que clicks dentro del panel cierren el modal (si backdrop usa delegación)
      const panel = modal ? modal.querySelector('.quiz-panel') : null;
      panel?.addEventListener('click', function(e){ e.stopPropagation(); });

      // Preguntas del cuestionario (render básico, accesible)
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

      const list = document.getElementById('quizQuestions');
      if(list){
        list.innerHTML = '';
        questions.forEach((q, i) => {
          const li = document.createElement('li');
          li.className = 'quiz-question';
          const yesId = `q${i}_yes`;
          const noId = `q${i}_no`;
          li.innerHTML = `
            <fieldset>
              <legend>${q}</legend>
              <label for="${yesId}"><input id="${yesId}" type="radio" name="q${i}" value="yes"> Sí</label>
              <label for="${noId}" style="margin-left:12px;"><input id="${noId}" type="radio" name="q${i}" value="no"> No</label>
            </fieldset>
          `;
          list.appendChild(li);
        });
      }

      // Lógica de resultado y reinicio
      const submit = document.getElementById('quizSubmit');
      const reset = document.getElementById('quizReset');
      const resultBox = document.getElementById('quizResult');

      submit?.addEventListener('click', function(e){
        e.preventDefault();
        if(!list || !resultBox) return;
        const answers = Array.from(list.querySelectorAll('input[type="radio"]:checked'));
        const yesCount = answers.filter(a => a.value === 'yes').length;
        resultBox.hidden = false;
        if(yesCount >= 4){
          resultBox.innerHTML = `<strong>Riesgo alto:</strong> Has respondido "Sí" a ${yesCount} preguntas. Considera buscar ayuda profesional.`;
        } else if(yesCount >= 2){
          resultBox.innerHTML = `<strong>Riesgo moderado:</strong> Has respondido "Sí" a ${yesCount} preguntas. Vigila la situación y consulta recursos de apoyo.`;
        } else {
          resultBox.innerHTML = `<strong>Riesgo bajo:</strong> Has respondido "Sí" a ${yesCount} preguntas. Si tienes dudas, consulta con un profesional.`;
        }
        resultBox.focus();
      });

      reset?.addEventListener('click', function(e){
        e.preventDefault();
        if(!list || !resultBox) return;
        list.querySelectorAll('input[type="radio"]').forEach(i => i.checked = false);
        resultBox.hidden = true;
        resultBox.innerHTML = '';
      });
    })();
    </script>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
    <script>anchors.add();</script>
  </body>
</html>
