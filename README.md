<<!doctype html>
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
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:'Inter',system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;color:#222;background:#fff;line-height:1.45}
    .hero-article{position:relative;width:100%;height:62vh;min-height:420px;overflow:hidden;display:block;cursor:pointer}
    .hero-img{width:100%;height:100%;object-fit:cover;display:block;transition:opacity .35s ease}
    .hero-overlay{position:absolute;inset:0;background:linear-gradient(135deg, rgba(11,61,145,0.55) 0%, rgba(0,0,0,0.25) 60%);pointer-events:none}
    .hero-text{position:absolute;top:6%;left:6%;right:6%;color:var(--white);text-shadow:0 6px 18px rgba(0,0,0,0.55);max-width:58%}
    .hero-title{margin:0 0 12px 0;font-weight:800;line-height:1.02;font-size:clamp(28px,4.6vw,56px);letter-spacing:-0.02em}
    .hero-sub{margin:0;font-weight:500;font-size:clamp(13px,1.6vw,20px);opacity:0.98}
    .hero-credit{position:absolute;right:4%;bottom:3%;font-size:12px;color:rgba(255,255,255,0.95);text-shadow:0 2px 6px rgba(0,0,0,0.6)}
    .container{max-width:1100px;margin:28px auto;padding:0 20px}
    .kicker{color:var(--muted);font-weight:600;margin-bottom:8px}
    .lead{font-size:18px;color:#111;margin:12px 0 20px}
    .meta{color:var(--muted);font-size:13px;margin-bottom:18px}
    h2{font-size:22px;margin:22px 0 12px}
    p{margin:0 0 14px}
    .two-col{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:start}
    .sidebar{background:#fafafa;padding:18px;border-radius:8px;border:1px solid #eee}
    .recuadro{background:#fff;border-left:4px solid var(--accent);padding:12px 14px;margin:14px 0;border-radius:4px}
    .pull{font-weight:700;font-size:20px;color:#111;margin:18px 0}
    .small{font-size:13px;color:var(--muted)}
    .toggle-hint{font-size:12px;color:rgba(255,255,255,0.9);margin-top:8px;opacity:0.95}
    @media (max-width:980px){
      .two-col{grid-template-columns:1fr}
      .hero-text{max-width:86%}
    }
    @media (max-width:600px){
      .hero-article{height:48vh;min-height:320px}
      .hero-title{font-size:clamp(20px,7.5vw,32px)}
      .hero-sub{font-size:14px}
      .hero-text{top:8%;left:6%;right:6%}
      .hero-credit{left:6%;right:auto;bottom:6%}
    }
    a:focus{outline:3px solid var(--blue);outline-offset:2px}
  </style>
</head>
<body>
  <!--
    Hero: haz clic sobre la portada para alternar entre apuestas.jpg y apuestas2.jpg (si existe).
    Asegúrate de subir ambas imágenes a la raíz del repositorio o ajustar rutas si están en una carpeta.
  -->
  <header id="hero" class="hero-article" role="img" aria-label="Portada de investigación: fachada de casino iluminada en Culiacán con silueta humana en primer plano.">
    <img id="heroImg" src="apuestas.jpg" alt="Fachada de casino iluminada en Culiacán con neón; silueta de una persona en primer plano y reflejos en pavimento húmedo" class="hero-img" />
    <div class="hero-overlay" aria-hidden="true"></div>

    <div class="hero-text">
      <h1 class="hero-title">Ludopatía y dinero sucio: cómo las máquinas, las apps y la opacidad regulatoria devoran a Sinaloa</h1>
      <p class="hero-sub"><strong>Investigación especial — Café Expresso Portal | Culiacán, Sinaloa</strong><br><em>La adicción al juego se alimenta de accesibilidad digital, vacíos regulatorios y presuntas redes financieras.</em></p>
      <div class="toggle-hint" id="toggleHint">Haz clic en la portada para ver la versión alternativa</div>
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
          <p>En la última década la oferta de juego en Sinaloa se multiplicó: salas de juego, minicasinos y plataformas


