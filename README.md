<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Café Expresso Portal — La ludopatía en Culiacán</title>
  <meta name="description" content="Investigación sobre la proliferación de apuestas y minicasinos en Culiacán: impacto social, testimonios y propuestas.">
  <link rel="canonical" href="https://ingenieroalfredomiranda.github.io/cafexpressoportal/">
  <meta property="og:type" content="article">
  <meta property="og:title" content="La ludopatía en Culiacán — Café Expresso Portal">
  <meta property="og:description" content="Investigación sobre la proliferación de apuestas y minicasinos en Culiacán: impacto social, testimonios y propuestas.">
  <meta property="og:url" content="https://ingenieroalfredomiranda.github.io/cafexpressoportal/">
  <meta property="og:site_name" content="Café Expresso Portal">
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="La ludopatía en Culiacán — Café Expresso Portal">
  <meta name="twitter:description" content="Investigación sobre la proliferación de apuestas y minicasinos en Culiacán: impacto social, testimonios y propuestas.">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;700&family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
  <meta name="theme-color" content="#b33a3a">

  <style>
    /* Variables y base */
    :root{
      --brand:#b33a3a;
      --bg:#ffffff;
      --muted:#6b6b6b;
      --text:#111111;
      --max-width:1100px;
      --radius:8px;
      --gap:20px;
      --base-font: clamp(0.95rem, 1.6vw, 1.05rem);
      --heading-font: "Merriweather", serif;
      --body-font: "Roboto", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:var(--body-font);
      font-size:var(--base-font);
      color:var(--text);
      background:var(--bg);
      line-height:1.6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    /* Skip link for keyboard users */
    .skip-link{
      position: absolute;
      left: -999px;
      top: auto;
      width: 1px;
      height: 1px;
      overflow: hidden;
    }
    .skip-link:focus{
      left: 12px;
      top: 12px;
      width: auto;
      height: auto;
      padding: 8px 12px;
      background:#000;
      color:#fff;
      z-index:1000;
      border-radius:4px;
    }

    /* Header */
    header{
      position:sticky;
      top:0;
      z-index:60;
      background:linear-gradient(180deg, #fff, #fff);
      border-bottom:1px solid #eee;
      backdrop-filter: blur(4px);
    }
    .header-inner{
      max-width:var(--max-width);
      margin:0 auto;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:var(--gap);
      padding:12px 16px;
    }
    .brand{
      display:flex;
      align-items:center;
      gap:12px;
      text-decoration:none;
      color:var(--text);
    }
    .brand img{height:44px;width:auto;display:block}
    .brand .title{font-weight:700;font-family:var(--heading-font);font-size:1.05rem}
    nav{display:flex;gap:14px;align-items:center}
    nav a{color:var(--text);text-decoration:none;font-weight:600;padding:8px;border-radius:6px}
    nav a:hover, nav a:focus{background:#fff0f0;outline:none}

    /* Menu toggle for small screens */
    .menu-toggle{
      display:none;
      background:none;
      border:0;
      font-size:20px;
      padding:8px;
      border-radius:6px;
    }

    /* Layout */
    main{max-width:var(--max-width);margin:28px auto;padding:0 16px}
    .article-grid{display:grid;grid-template-columns:2fr 1fr;gap:28px;align-items:start}
    article h1{font-family:var(--heading-font);font-size:clamp(1.4rem, 3.2vw, 2rem);margin:0 0 8px}
    .meta{color:var(--muted);font-size:0.95rem;margin-bottom:12px}
    .lead{font-family:var(--heading-font);color:var(--muted);margin-bottom:16px}
    figure{margin:0}
    figure img{width:100%;height:auto;border-radius:var(--radius);display:block}
    figcaption{color:var(--muted);font-size:0.9rem;margin-top:8px}

    h2{font-family:var(--heading-font);margin-top:20px;margin-bottom:8px}
    blockquote{
      border-left:4px solid var(--brand);
      background:#fff8f8;
      padding:12px 16px;
      margin:16px 0;
      border-radius:6px;
      color:var(--text);
    }

    ul{padding-left:1.1rem}
    .share{display:flex;gap:8px;margin-top:14px;flex-wrap:wrap}
    .btn{
      display:inline-flex;align-items:center;gap:8px;
      background:var(--brand);color:#fff;padding:8px 12px;border-radius:6px;text-decoration:none;font-weight:600;border:0;cursor:pointer
    }
    .btn.secondary{background:#f5f5f5;color:var(--text);border:1px solid #eee}

    aside{background:#fafafa;padding:16px;border-radius:8px;border:1px solid #f0f0f0}
    aside h3{margin-top:0}
    footer{
      margin-top:40px;background:#111;color:#fff;padding:20px 16px;text-align:center;font-size:0.95rem
    }

    /* Accessibility focus */
    a:focus, button:focus, input:focus, textarea:focus{
      outline:3px solid #ffd1d1;outline-offset:3px;
    }

    /* Responsive */
    @media (max-width:900px){
      .article-grid{grid-template-columns:1fr}
      nav{display:none;position:absolute;left:0;right:0;top:64px;background:var(--bg);flex-direction:column;padding:12px;border-bottom:1px solid #eee}
      .menu-toggle{display:block}
      .menu-open nav{display:flex}
      .header-inner{position:relative}
    }

    /* Reduced motion */
    @media (prefers-reduced-motion: reduce){
      *{transition:none!important}
    }
  </style>
</head>
<body>
  <a class="skip-link" href="#main">Saltar al contenido</a>

  <header>
    <div class="header-inner" id="headerInner">
      <a class="brand" href="/" aria-label="Café Expresso Portal - Inicio">
        <!-- Reemplaza logo.svg por tu logo vectorial optimizado -->
        <img src="logo.svg" alt="Logotipo Café Expresso Portal" width="44" height="44">
        <div>
          <div class="title">Café Expresso Portal</div>
          <div style="font-size:0.85rem;color:var(--muted)">Periodismo de investigación</div>
        </div>
      </a>

      <button class="menu-toggle" aria-controls="main-nav" aria-expanded="false" aria-label="Abrir menú">☰</button>

      <nav id="main-nav" role="navigation" aria-label="Menú principal">
        <a href="/">Inicio</a>
        <a href="/reportajes">Reportajes</a>
        <a href="/opinion">Opinión</a>
        <a href="/contacto">Contacto</a>
      </nav>
    </div>
  </header>

  <main id="main" role="main">
    <article aria-labelledby="titulo">
      <h1 id="titulo">La ludopatía en Culiacán: una adicción que devora hogares</h1>
      <div class="meta">
        <strong>Miguel Alfredo Miranda Félix</strong> • <time id="published" datetime="">12 enero 2026</time>
      </div>

      <p class="lead">Investigación sobre la proliferación de maquinitas y plataformas de apuestas en Culiacán, su impacto en jóvenes y familias, y las propuestas para mitigarlo.</p>

      <div class="article-grid">
        <div>
          <figure>
            <!-- Imágenes responsivas: reemplaza los archivos por tus versiones optimizadas -->
            <img
              src="ludopatia-culiacan-800.jpg"
              srcset="ludopatia-culiacan-480.jpg 480w, ludopatia-culiacan-800.jpg 800w, ludopatia-culiacan-1200.jpg 1200w"
              sizes="(max-width:600px) 100vw, (max-width:900px) 90vw, 800px"
              alt="Máquinas de apuestas en un local de Culiacán"
              loading="lazy"
              width="1200" height="675">
            <figcaption>Minicasinos y maquinitas en Culiacán; foto de archivo.</figcaption>
          </figure>

          <h2>Magnitud del problema</h2>
          <p>Estudios y entrevistas indican que entre <strong>1% y 3%</strong> de la población puede presentar ludopatía, con mayor incidencia en jóvenes de 18 a 25 años.</p>

          <blockquote>“La ludopatía es un asesino silencioso” — Testimonio de un miembro de Jugadores Anónimos</blockquote>

          <h2>Factores de riesgo</h2>
          <ul>
            <li>Antecedentes familiares de adicción o violencia.</li>
            <li>Normalización del juego en espacios públicos y digitales.</li>
            <li>Contextos económicos precarios que incentivan la búsqueda de ingresos rápidos.</li>
            <li>Problemas de salud mental como ansiedad y depresión.</li>
          </ul>

          <h2>Consecuencias sociales</h2>
          <p>Ruptura familiar, endeudamiento, pérdida de patrimonio y riesgo de delitos para financiar apuestas.</p>

          <h2>Propuestas</h2>
          <ul>
            <li>Campañas de prevención en escuelas y universidades.</li>
            <li>Regulación con límites automáticos y auditorías públicas.</li>
            <li>Programas de atención y rehabilitación accesibles y gratuitos.</li>
          </ul>

          <div class="share" role="group" aria-label="Compartir artículo">
            <button class="btn" id="copyLink">Copiar enlace</button>
            <a class="btn secondary" href="#" id="shareTwitter" aria-label="Compartir en Twitter">Twitter</a>
            <a class="btn secondary" href="#" id="shareFacebook" aria-label="Compartir en Facebook">Facebook</a>
          </div>
        </div>

        <aside aria-labelledby="asideTitle">
          <h3 id="asideTitle">Datos clave</h3>
          <p class="meta">Mercado estimado: <strong>50,000 millones de pesos</strong></p>

          <h4>Contacto editorial</h4>
          <p><a href="mailto:editor@cafexpressoportal.mx">editor@cafexpressoportal.mx</a></p>

          <h4>Recursos</h4>
          <ul>
            <li><a href="#" rel="noopener">Ley de Juegos y Sorteos (resumen)</a></li>
            <li><a href="#" rel="noopener">Guía de prevención para escuelas</a></li>
          </ul>

          <h4>Suscríbete</h4>
          <form id="newsletter" onsubmit="event.preventDefault(); alert('Gracias por suscribirte');" aria-label="Formulario de suscripción">
            <label for="email" class="sr-only">Correo electrónico</label>
            <input id="email" type="email" placeholder="Tu correo" required style="width:100%;padding:8px;margin-top:8px;border-radius:6px;border:1px solid #e6e6e6">
            <button class="btn" type="submit" style="width:100%;margin-top:8px">Suscribirme</button>
          </form>
        </aside>
      </div>
    </article>
  </main>

  <footer role="contentinfo">
    <div style="max-width:var(--max-width);margin:0 auto;padding:0 16px">
      <p style="margin:0 0 8px">© <strong>Café Expresso Portal</strong> • Política editorial • Aviso de privacidad</p>
      <p style="margin:0;font-size:0.9rem;color:#cfcfcf">Diseño y desarrollo: equipo editorial</p>
    </div>
  </footer>

  <script>
    // --- Menú responsive accesible ---
    (function(){
      const header = document.getElementById('headerInner');
      const btn = document.querySelector('.menu-toggle');
      const nav = document.getElementById('main-nav');

      function closeNavOnLarge() {
        if (window.innerWidth > 900) {
          header.classList.remove('menu-open');
          nav.style.display = 'flex';
          btn.setAttribute('aria-expanded','false');
        } else {
          nav.style.display = '';
          btn.setAttribute('aria-expanded','false');
        }
      }

      btn.addEventListener('click', function(){
        const isOpen = header.classList.toggle('menu-open');
        btn.setAttribute('aria-expanded', String(isOpen));
        // Ensure nav is visible when open on small screens
        if(isOpen) nav.style.display = 'flex';
        else nav.style.display = '';
      });

      window.addEventListener('resize', closeNavOnLarge);
      document.addEventListener('DOMContentLoaded', closeNavOnLarge);
    })();

    // --- Copiar enlace y compartir ---
    (function(){
      const copyBtn = document.getElementById('copyLink');
      copyBtn.addEventListener('click', async function(){
        try {
          await navigator.clipboard.writeText(location.href);
          copyBtn.textContent = 'Enlace copiado';
          setTimeout(()=> copyBtn.textContent = 'Copiar enlace', 2000);
        } catch(e){
          alert('No se pudo copiar el enlace. Usa Ctrl+C para copiar la URL.');
        }
      });

      const twitter = document.getElementById('shareTwitter');
      twitter.addEventListener('click', function(e){
        e.preventDefault();
        const text = encodeURIComponent(document.title);
        const url = encodeURIComponent(location.href);
        window.open(`https://twitter.com/intent/tweet?text=${text}&url=${url}`, '_blank', 'noopener');
      });

      const fb = document.getElementById('shareFacebook');
      fb.addEventListener('click', function(e){
        e.preventDefault();
        const url = encodeURIComponent(location.href);
        window.open(`https://www.facebook.com/sharer/sharer.php?u=${url}`, '_blank', 'noopener');
      });
    })();

    // --- JSON-LD dinámico con fecha de publicación actualizada ---
    (function(){
      const publishedEl = document.getElementById('published');
      const now = new Date();
      // Ajusta la fecha aquí si necesitas la fecha real del artículo
      const publishedDate = new Date('2026-01-12T00:00:00Z');
      publishedEl.textContent = publishedDate.toLocaleDateString('es-MX', { day:'numeric', month:'long', year:'numeric' });
      publishedEl.setAttribute('datetime', publishedDate.toISOString());

      const jsonLd = {
        "@context": "https://schema.org",
        "@type": "NewsArticle",
        "headline": "La ludopatía en Culiacán: una adicción que devora hogares",
        "image": [
          "https://ingenieroalfredomiranda.github.io/cafexpressoportal/ludopatia-culiacan-1200.jpg"
        ],
        "datePublished": publishedDate.toISOString(),
        "author": {
          "@type": "Person",
          "name": "Miguel Alfredo Miranda Félix"
        },
        "publisher": {
          "@type": "Organization",
          "name": "Café Expresso Portal",
          "logo": {
            "@type": "ImageObject",
            "url": "https://ingenieroalfredomiranda.github.io/cafexpressoportal/logo.svg"
          }
        },
        "description": "Investigación sobre la proliferación de maquinitas y plataformas de apuestas en Culiacán, su impacto en jóvenes y familias, y las propuestas para mitigarlo."
      };

      const script = document.createElement('script');
      script.type = 'application/ld+json';
      script.text = JSON.stringify(jsonLd);
      document.head.appendChild(script);
    })();

    // --- Mejora progresiva: detecta si navigator.share está disponible ---
    (function(){
      if (navigator.share) {
        const shareBtn = document.createElement('button');
        shareBtn.className = 'btn';
        shareBtn.textContent = 'Compartir';
        shareBtn.style.marginLeft = '8px';
        document.querySelector('.share').appendChild(shareBtn);
        shareBtn.addEventListener('click', async () => {
          try {
            await navigator.share({ title: document.title, text: document.querySelector('.lead').textContent, url: location.href });
          } catch (err) {
            // usuario canceló o no se pudo compartir
          }
        });
      }
    })();
  </script>
</body>
</html>
