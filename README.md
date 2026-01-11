<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>La Ludopatía en Culiacán — Investigación</title>

  <!-- Tipografías -->
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
      line-height:1.55;
    }
    .container{
      max-width:var(--max-width);
      margin:32px auto;
      padding:0 20px;
    }
    .masthead{
      display:flex;
      align-items:flex-end;
      gap:20px;
      border-bottom:1px solid #e6e6e6;
      padding-bottom:18px;
      margin-bottom:22px;
    }
    .brand{
      display:flex;
      align-items:center;
      gap:14px;
    }
    .brand .logo{
      width:86px;
      height:86px;
      background:#111;
      color:#fff;
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:700;
      font-family:var(--serif);
      font-size:20px;
      letter-spacing:1px;
    }
    .brand .title{
      font-family:var(--serif);
      font-size:20px;
      line-height:1;
      color:var(--text);
    }
    .brand .subtitle{
      font-size:12px;
      color:var(--muted);
      margin-top:4px;
    }
    .meta{
      margin-left:auto;
      text-align:right;
      color:var(--muted);
      font-size:13px;
    }
    .hero{
      display:grid;
      grid-template-columns: 1fr 380px;
      gap:28px;
      align-items:start;
      margin-bottom:28px;
    }
    .hero-main{
      background:#fafafa;
      padding:22px;
      border-radius:6px;
      box-shadow:0 6px 18px rgba(15,15,15,0.04);
    }
    .kicker{
      display:inline-block;
      color:var(--accent);
      font-weight:700;
      font-size:13px;
      letter-spacing:0.6px;
      margin-bottom:10px;
      text-transform:uppercase;
    }
    .headline{
      font-family:var(--serif);
      font-size:34px;
      margin:6px 0 12px 0;
      line-height:1.08;
      color:var(--text);
    }
    .standfirst{
      color:var(--muted);
      font-size:16px;
      margin-bottom:16px;
    }
    .byline{
      font-size:13px;
      color:var(--muted);
      margin-bottom:14px;
    }
    .hero-image{
      width:100%;
      height:360px;
      background:#ddd;
      border-radius:6px;
      overflow:hidden;
      display:flex;
      align-items:flex-end;
      justify-content:flex-start;
      position:relative;
    }
    .hero-image img{
      width:100%;
      height:100%;
      object-fit:cover;
      display:block;
    }
    .hero-caption{
      position:absolute;
      left:12px;
      bottom:12px;
      background:rgba(0,0,0,0.55);
      color:#fff;
      padding:10px 12px;
      font-size:13px;
      border-radius:4px;
      max-width:85%;
      font-family:var(--sans);
    }
    .side{
      display:flex;
      flex-direction:column;
      gap:18px;
    }
    .card{
      background:#fff;
      border-radius:6px;
      padding:14px;
      box-shadow:0 6px 18px rgba(15,15,15,0.03);
      border:1px solid #f0f0f0;
    }
    .card h4{margin:0 0 8px 0;font-size:15px;font-family:var(--serif)}
    .card p{margin:0;color:var(--muted);font-size:13px}
    .article{
      display:grid;
      grid-template-columns: 1fr 320px;
      gap:28px;
      margin-top:18px;
    }
    .article-main{
      font-size:16px;
      color:var(--text);
    }
    .article-main h2{
      font-family:var(--serif);
      font-size:22px;
      margin-top:28px;
      margin-bottom:10px;
    }
    .article-main p{margin:0 0 14px 0; color:var(--text);}
    .pull-quote{
      font-family:var(--serif);
      font-size:20px;
      color:var(--accent);
      border-left:4px solid var(--accent);
      padding:12px 16px;
      margin:18px 0;
      background:#fff8f8;
    }
    .testimonios{
      display:grid;
      grid-template-columns: repeat(3,1fr);
      gap:14px;
      margin:18px 0 26px 0;
    }
    .testimonio{
      background:#111;
      color:#fff;
      padding:0;
      border-radius:6px;
      position:relative;
      min-height:160px;
      overflow:hidden;
      display:flex;
      flex-direction:column;
      justify-content:flex-end;
    }
    .testimonio a{
      color:inherit;
      text-decoration:none;
      display:block;
      height:100%;
      width:100%;
    }
    .testimonio .overlay{
      padding:16px;
      background:linear-gradient(180deg, rgba(0,0,0,0.0) 0%, rgba(0,0,0,0.65) 60%);
      display:flex;
      flex-direction:column;
      justify-content:flex-end;
      height:100%;
    }
    .testimonio .quote{
      font-family:var(--serif);
      font-size:16px;
      margin-bottom:8px;
      color:#fff;
    }
    .testimonio .credit{
      font-size:12px;
      color:#ddd;
      opacity:0.95;
    }
    .testimonio .hook{
      position:absolute;
      right:12px;
      top:12px;
      background:rgba(255,255,255,0.08);
      padding:6px 8px;
      border-radius:4px;
      font-size:12px;
      color:#fff;
      font-weight:600;
    }
    .testimonio img{
      position:absolute;
      inset:0;
      width:100%;
      height:100%;
      object-fit:cover;
      display:block;
      filter:contrast(0.95) saturate(0.9);
    }
    .sidebar{
      position:sticky;
      top:24px;
      align-self:start;
      display:flex;
      flex-direction:column;
      gap:14px;
    }
    .sidebar .box{padding:12px;border-radius:6px;background:#fff;border:1px solid #f0f0f0}
    .sidebar h5{margin:0 0 8px 0;font-family:var(--serif);font-size:15px}
    .sidebar p{margin:0;color:var(--muted);font-size:13px}
    .photo-credit{
      display:block;
      font-size:12px;
      color:var(--muted);
      margin-top:8px;
    }
    footer{
      margin-top:36px;
      padding-top:22px;
      border-top:1px solid #e6e6e6;
      color:var(--muted);
      font-size:13px;
    }
    @media (max-width:980px){
      .hero{grid-template-columns:1fr; }
      .hero-main{order:2}
      .hero-image{order:1;height:260px}
      .article{grid-template-columns:1fr}
      .testimonios{grid-template-columns:1fr}
      .container{padding:0 16px}
    }
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

        <p style="color:var(--muted);font-size:14px;margin-top:6px;">
          Resumen: Este reportaje documenta factores de riesgo, trayectorias clínicas, impacto económico y vínculos con lavado de dinero en Sinaloa. Incluye testimonios, solicitudes de información y propuestas de política pública.
        </p>
      </article>

      <aside class="side" aria-label="Portada y destacados">
        <figure class="hero-image" role="img" aria-label="Portada principal">
          <!-- Portada: imagen central 'apuestas' alojada en GitHub Pages -->
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas.jpg" alt="Portada: Mano contando billetes; fondo nocturno con letreros de apuestas y silueta de espaldas">
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

    <!-- Article body -->
    <main class="article" role="main">
      <section class="article-main">
        <h2>Contexto: de entretenimiento a dependencia</h2>
        <p>La ludopatía, o trastorno por juego, es una adicción sin sustancia que afecta a miles de personas en México. En Culiacán, la proliferación de casinos, minicasinos y plataformas digitales ha facilitado el acceso al juego, especialmente entre adolescentes y jóvenes universitarios.</p>

        <p>Investigaciones locales y nacionales estiman que entre <strong>1% y 3%</strong> de la población puede presentar problemas de juego; en entornos con precariedad económica, la búsqueda de ingresos rápidos agrava el riesgo.</p>

        <div class="pull-quote">“La ludopatía es un asesino silencioso que te lleva a la cárcel, a la locura o a la muerte.” — Testimonio recogido en Culiacán</div>

        <h2 id="testimonios">Testimonios que atrapan</h2>

        <!-- Testimonios con imágenes vinculadas a secciones internas -->
        <div class="testimonios" aria-label="Testimonios destacados">
          <!-- Testimonio 1: Impacto social -->
          <div class="testimonio" role="article" aria-labelledby="t1">
            <a href="#detalle-impacto-social" title="Abrir testimonio: Impacto social">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas_supervivencia.jpg" alt="Manos intercambiando un sobre con billetes; fondo nocturno con letreros de apuestas">
              <div class="overlay">
                <div class="quote">“Apostadores llegan hasta a prostituirse.”</div>
                <div class="credit">Publicación local; relato de supervivencia económica</div>
              </div>
            </a>
            <div class="hook">Impacto social</div>
          </div>

          <!-- Testimonio 2: Toque humano -->
          <div class="testimonio" role="article" aria-labelledby="t2">
            <a href="#detalle-toque-humano" title="Abrir testimonio: Toque humano">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino_mentira_espejo.jpg" alt="Mesa con fichas y billetes; espejo agrietado que refleja luces de neón">
              <div class="overlay">
                <div class="quote">“El casino es una mentira: no se hizo para perder, sino para que los dueños ganen.”</div>
                <div class="credit">Caso clínico; Los Mochis</div>
              </div>
            </a>
            <div class="hook">Toque humano</div>
          </div>

          <!-- Testimonio 3: Pérdida económica -->
          <div class="testimonio" role="article" aria-labelledby="t3">
            <a href="#detalle-perdida-economica" title="Abrir testimonio: Pérdida económica">
              <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/perdida_economica_caja.jpg" alt="Caja de mudanza abierta frente a una puerta cerrada; objetos personales dispersos">
              <div class="overlay">
                <div class="quote">“He perdido fácil más de dos millones de pesos.”</div>
                <div class="credit">Testimonio personal; recuperación parcial</div>
              </div>
            </a>
            <div class="hook">Pérdida económica</div>
          </div>
        </div>

        <h2 id="detalle-impacto-social">Impacto social — Testimonio ampliado</h2>
        <p>Relato ampliado: en comunidades con precariedad económica, la presión por obtener recursos rápidos empuja a algunas personas a medidas extremas. Este testimonio documenta cómo la deuda y la estigmatización empujan a la marginalidad y a prácticas de supervivencia que dañan a familias enteras.</p>

        <figure style="margin:18px 0;">
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino2.jpg" alt="Interior de un casino o maquinitas en Culiacán" style="width:100%;height:auto;border-radius:6px;display:block;">
          <figcaption class="photo-credit">Maquinitas en colonias populares; la accesibilidad normaliza el juego. Foto: archivo local</figcaption>
        </figure>

        <h2 id="detalle-toque-humano">Toque humano — Caso clínico (Los Mochis)</h2>
        <p>Relato clínico: la progresión desde el juego recreativo hasta el trastorno por juego puede incluir convulsiones por estrés, intentos autolesivos y pérdida de empleo. Este caso muestra la necesidad de protocolos de derivación entre servicios de salud y redes comunitarias.</p>

        <figure style="margin:18px 0;">
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino3.webp" alt="Exterior de un minicasino en Culiacán" style="width:100%;height:auto;border-radius:6px;display:block;">
          <figcaption class="photo-credit">Minicasinos en zonas urbanas; a menudo operan cerca de áreas residenciales. Foto: archivo local</figcaption>
        </figure>

        <h2 id="detalle-perdida-economica">Pérdida económica — Testimonio ampliado</h2>
        <p>Relato económico: la pérdida de patrimonio y el endeudamiento masivo son consecuencias frecuentes. En este testimonio, la persona describe el uso de tarjetas, préstamos y la venta de bienes para sostener la conducta adictiva, así como el proceso de recuperación parcial.</p>

        <figure style="margin:18px 0;">
          <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/casino4.png" alt="Documentos y extractos bancarios sobre una mesa" style="width:100%;height:auto;border-radius:6px;display:block;">
          <figcaption class="photo-credit">Extractos y documentos que muestran el rastro financiero de la adicción. Foto: archivo local</figcaption>
        </figure>

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

  <!-- Script ligero para asegurar carga de imágenes remotas y fallback -->
  <script>
    (function(){
      const fallback = "data:image/svg+xml;charset=UTF-8," + encodeURIComponent(
        '<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="800"><rect width="100%" height="100%" fill="#e9e9e9"/><text x="50%" y="50%" font-family="Arial, sans-serif" font-size="20" fill="#777" text-anchor="middle">Imagen pendiente</text></svg>'
      );

      document.querySelectorAll('img').forEach(img=>{
        img.addEventListener('error', function(){ this.src = fallback; });
      });

      // Smooth scroll for anchor links (enhances UX when clicking testimonios)
      document.querySelectorAll('a[href^="#"]').forEach(a=>{
        a.addEventListener('click', function(e){
          const targetId = this.getAttribute('href').slice(1);
          const target = document.getElementById(targetId);
          if(target){
            e.preventDefault();
            target.scrollIntoView({behavior:'smooth', block:'start'});
            // add a subtle focus for accessibility
            target.setAttribute('tabindex','-1');
            target.focus({preventScroll:true});
          }
        });
      });
    })();
  </script>
</body>
</html>

