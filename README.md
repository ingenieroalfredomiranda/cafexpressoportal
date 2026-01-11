<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Café Expresso Portal — Reportajes</title>
  <meta name="description" content="Reportajes de investigación sobre ludopatía en Culiacán y temas sociales.">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;700&family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
  <meta name="theme-color" content="#2b2b2b">
  <script type="application/ld+json">
  {
    "@context":"https://schema.org",
    "@type":"NewsArticle",
    "headline":"La ludopatía en Culiacán",
    "author":{"@type":"Person","name":"Miguel Alfredo Miranda Félix"},
    "publisher":{"@type":"Organization","name":"Café Expresso Portal"},
    "datePublished":"2025-01-01"
  }
  </script>
  <style>
    :root{
      --brand:#b33a3a; --accent:#f5f5f5; --text:#222; --muted:#666;
      font-family: Roboto, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{margin:0;color:var(--text);background:#fff;line-height:1.6}
    header{display:flex;align-items:center;justify-content:space-between;padding:12px 20px;background:#fff;border-bottom:1px solid #eee;position:sticky;top:0;z-index:50}
    .logo{display:flex;align-items:center;gap:10px}
    .logo img{height:44px}
    nav{display:flex;gap:16px}
    nav a{color:var(--text);text-decoration:none;font-weight:600}
    .container{max-width:1100px;margin:24px auto;padding:0 16px}
    .lead{font-family:Merriweather, serif;font-size:1.15rem;color:var(--muted);margin-bottom:12px}
    .grid{display:grid;grid-template-columns:2fr 1fr;gap:24px}
    article img{max-width:100%;height:auto;border-radius:6px}
    .meta{color:var(--muted);font-size:0.95rem;margin-bottom:8px}
    blockquote{border-left:4px solid var(--brand);padding:12px 16px;background:#fff8f8;margin:16px 0}
    footer{background:#111;color:#fff;padding:20px;text-align:center;margin-top:40px}
    /* Responsive */
    @media(max-width:900px){.grid{grid-template-columns:1fr}nav{display:none} .menu-toggle{display:block}}
    .menu-toggle{display:none;background:none;border:0;font-size:18px}
    .share{display:flex;gap:8px;margin-top:12px}
    .btn{background:var(--brand);color:#fff;padding:8px 12px;border-radius:4px;text-decoration:none}
    /* Accessibility */
    a:focus{outline:3px solid #ffd1d1;outline-offset:2px}
  </style>
</head>
<body>
  <header>
    <div class="logo">
      <img src="logo.svg" alt="Café Expresso Portal logo">
      <div>
        <strong>Café Expresso Portal</strong><br><small style="color:var(--muted)">Periodismo de investigación</small>
      </div>
    </div>
    <button class="menu-toggle" aria-controls="main-nav" aria-expanded="false">☰</button>
    <nav id="main-nav" role="navigation" aria-label="Menú principal">
      <a href="/">Inicio</a>
      <a href="/reportajes">Reportajes</a>
      <a href="/opinion">Opinión</a>
      <a href="/contacto">Contacto</a>
    </nav>
  </header>

  <main class="container" role="main">
    <article aria-labelledby="titulo">
      <h1 id="titulo">La ludopatía en Culiacán una adicción que devora hogares</h1>
      <div class="meta">Por <strong>Miguel Alfredo Miranda Félix</strong> • 12 enero 2026</div>
      <p class="lead">Resumen breve que atrapa al lector y resume el hallazgo principal en una o dos líneas.</p>
      <div class="grid">
        <div>
          <figure>
            <img src="ludopatia-culiacan.jpg" alt="Máquinas de apuestas en Culiacán" loading="lazy" width="1200" height="675">
            <figcaption style="color:var(--muted);font-size:0.9rem">Minicasinos en Culiacán; foto de archivo.</figcaption>
          </figure>

          <h2>Magnitud del problema</h2>
          <p><strong>1%–3% de la población</strong> presenta ludopatía; los jóvenes de 18 a 25 años son los más afectados.</p>

          <blockquote>“La ludopatía es un asesino silencioso” — Testimonio de Jugadores Anónimos</blockquote>

          <h2>Propuestas</h2>
          <ul>
            <li><strong>Prevención</strong> en escuelas y universidades.</li>
            <li><strong>Regulación</strong> con auditorías públicas y límites automáticos.</li>
            <li><strong>Atención</strong> con programas gratuitos y capacitación médica.</li>
          </ul>

          <div class="share" aria-hidden="false">
            <a class="btn" href="#" onclick="navigator.clipboard.writeText(location.href);return false">Copiar enlace</a>
            <a class="btn" href="#" aria-label="Compartir en Twitter">Twitter</a>
          </div>
        </div>

        <aside>
          <h3>Datos clave</h3>
          <p class="meta">Mercado estimado en 50,000 millones de pesos</p>
          <h4>Contacto</h4>
          <p><a href="mailto:editor@cafexpressoportal.mx">editor@cafexpressoportal.mx</a></p>
        </aside>
      </div>
    </article>
  </main>

  <footer>
    <small>© Café Expresso Portal • Política editorial • Aviso de privacidad</small>
  </footer>

  <script>
    // Menú responsive simple
    const btn = document.querySelector('.menu-toggle');
    const nav = document.getElementById('main-nav');
    btn?.addEventListener('click', () => {
      const expanded = btn.getAttribute('aria-expanded') === 'true';
      btn.setAttribute('aria-expanded', String(!expanded));
      nav.style.display = expanded ? 'none' : 'flex';
    });
  </script>
</body>
</html>
