<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Café Expresso Portal — La Ludopatía en Culiacán</title>
  <meta name="description" content="Reportaje especial: La ludopatía en Culiacán. Investigación sobre causas, consecuencias y vínculos con lavado de dinero." />
  <style>
    :root{
      --bg:#ffffff; --muted:#6b7280; --accent:#0a57ff; --card:#f8fafc; --border:#e6e9ef;
      --maxw:1100px; --gap:1rem;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:var(--bg);color:#0f172a;line-height:1.5}
    a{color:var(--accent);text-decoration:none}
    header{border-bottom:1px solid var(--border);background:#fff;position:sticky;top:0;z-index:20}
    .container{max-width:var(--maxw);margin:0 auto;padding:1rem}
    .topbar{display:flex;align-items:center;justify-content:space-between;padding:.5rem 0}
    .brand{display:flex;align-items:center;gap:.75rem}
    .brand .logo{width:44px;height:44px;background:#111;border-radius:6px;color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700}
    nav ul{display:flex;gap:1rem;list-style:none;margin:0;padding:0;font-weight:600;color:var(--muted)}
    nav a{color:var(--muted);padding:.5rem;border-radius:6px}
    nav a:hover{background:var(--card);color:#0b1220}

    main{display:grid;grid-template-columns: 1fr 320px;gap:1.25rem;padding:1.25rem 0}
    .hero{background:linear-gradient(180deg, rgba(10,87,255,0.06), transparent);padding:1rem;border-radius:8px;border:1px solid var(--border)}
    .hero img{width:100%;height:300px;object-fit:cover;border-radius:6px}
    .hero h1{margin:.5rem 0 0;font-size:1.6rem}
    .hero p{color:var(--muted);margin:.5rem 0 1rem}

    .grid{display:grid;grid-template-columns:repeat(2,1fr);gap:1rem;margin-top:1rem}
    .card{background:#fff;border:1px solid var(--border);padding:.85rem;border-radius:8px}
    .card h3{margin:.25rem 0;font-size:1rem}
    .card p{margin:.5rem 0;color:var(--muted);font-size:.95rem}

    aside{position:relative}
    .side-card{background:#fff;border:1px solid var(--border);padding:1rem;border-radius:8px;margin-bottom:1rem}
    .side-card h4{margin:0 0 .5rem;font-size:1rem}
    .small-list{display:flex;flex-direction:column;gap:.5rem}
    .small-list a{display:block;color:#0b1220;padding:.35rem 0;border-bottom:1px dashed #eef2f7}

    table{width:100%;border-collapse:collapse;margin-top:.5rem}
    th,td{padding:.5rem;border:1px solid #eef2f7;text-align:left;font-size:.95rem}
    th{background:#fbfdff;font-weight:700}

    footer{border-top:1px solid var(--border);padding:1rem 0;margin-top:1.5rem;background:#fff}
    .meta{font-size:.9rem;color:var(--muted)}

    /* Galería / Carrusel */
    .gallery-section{display:grid;gap:1rem;margin-top:1rem}
    .hero-figure{margin:0}
    .hero-figure img{width:100%;height:360px;object-fit:cover;border-radius:6px}
    .carousel{position:relative;overflow:hidden}
    .carousel-track{display:flex;gap:0.75rem;transition:transform .35s ease}
    .slide{min-width:260px;flex:0 0 auto;border-radius:6px;overflow:hidden;background:#fff;border:1px solid #eef2f7}
    .slide img{width:100%;height:160px;object-fit:cover;display:block}
    .slide figcaption{font-size:.9rem;color:#555;padding:.5rem}
    .carousel-btn{position:absolute;top:50%;transform:translateY(-50%);background:rgba(255,255,255,.95);border:1px solid #e6e9ef;padding:.5rem .6rem;border-radius:6px;cursor:pointer}
    .carousel-btn.prev{left:.5rem}
    .carousel-btn.next{right:.5rem}
    @media (max-width:980px){
      main{grid-template-columns:1fr; padding:1rem}
      .hero-figure img{height:220px}
      .slide{min-width:200px}
    }
  </style>
</head>
<body>
  <header>
    <div class="container topbar">
      <div class="brand">
        <div class="logo" aria-hidden="true">CE</div>
        <div>
          <div style="font-weight:800">Café Expresso Portal</div>
          <div style="font-size:.85rem;color:var(--muted)">Investigación · Culiacán, Sinaloa</div>
        </div>
      </div>

      <nav aria-label="Navegación principal">
        <ul>
          <li><a href="#">México</a></li>
          <li><a href="#">Investigación</a></li>
          <li><a href="#">Sociedad</a></li>
          <li><a href="#">Economía</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <div class="container">
    <main>
      <section>
        <!-- Hero / Artículo principal -->
        <article class="hero" aria-labelledby="hero-title">
          <figure class="hero-figure">
            <!-- REEMPLAZAR_SRC_IMAGEN_HERO: pega aquí la ruta que tu editor asignó a la imagen destacada -->
            <img src="REEMPLAZAR_SRC_IMAGEN_HERO" alt="Persona frente a un letrero de casino iluminado; simboliza la atracción del juego" />
            <figcaption style="font-size:.9rem;color:var(--muted);margin-top:.5rem">Crédito foto: Investigaciones Café Expresso Portal</figcaption>
          </figure>

          <h1 id="hero-title">La Ludopatía en Culiacán: Una Adicción Silenciosa</h1>
          <p><strong>Investigación especial</strong> — Reportaje que explora causas, consecuencias y vínculos con lavado de dinero en Sinaloa. Por Miguel Alfredo Miranda Félix · Enero 2026</p>
          <p class="meta">Resumen: La proliferación de casinos, minicasinos y plataformas digitales ha normalizado el juego y aumentado la vulnerabilidad de adolescentes y jóvenes.</p>
          <p><a href="#reportaje-completo">Leer reportaje completo</a></p>
        </article>

        <!-- Galería / Carrusel -->
        <section class="gallery-section" aria-label="Galería de imágenes sobre ludopatía">
          <div class="card">
            <h3>Galería: ambientes de juego</h3>
            <p class="meta">Imágenes que ilustran la presencia de máquinas, minicasinos y señales de riesgo en barrios urbanos.</p>
          </div>

          <div class="carousel card" aria-roledescription="carrusel">
            <button class="carousel-btn prev" aria-label="Anterior">‹</button>

            <div class="carousel-track" role="list">
              <!-- REEMPLAZAR_SRC_IMAGEN_1 -->
              <figure class="slide" role="listitem">
                <img src="REEMPLAZAR_SRC_IMAGEN_1" alt="Máquinas tragamonedas con luces y botones" loading="lazy" />
                <figcaption>Máquinas y minicasinos en barrios urbanos.</figcaption>
              </figure>

              <!-- REEMPLAZAR_SRC_IMAGEN_2 -->
              <figure class="slide" role="listitem">
                <img src="REEMPLAZAR_SRC_IMAGEN_2" alt="Sala de juego con iluminación tenue y fichas" loading="lazy" />
                <figcaption>Espacios que pueden servir como fachadas para operaciones financieras irregulares.</figcaption>
              </figure>

              <!-- REEMPLAZAR_SRC_IMAGEN_3 -->
              <figure class="slide" role="listitem">
                <img src="REEMPLAZAR_SRC_IMAGEN_3" alt="Billetes y tarjeta junto a un aviso sobre apuestas clandestinas" loading="lazy" />
                <figcaption>Apuestas clandestinas y videojuegos con máquinas de ficha.</figcaption>
              </figure>

              <!-- REEMPLAZAR_SRC_IMAGEN_4 -->
              <figure class="slide" role="listitem">
                <img src="REEMPLAZAR_SRC_IMAGEN_4" alt="Persona jugando en una mesa de apuestas; contexto testimonial" loading="lazy" />
                <figcaption>Testimonio: “La ludopatía es un asesino silencioso…”</figcaption>
              </figure>
            </div>

            <button class="carousel-btn next" aria-label="Siguiente">›</button>
          </div>
        </section>

        <!-- Rejilla de artículos relacionados -->
        <div class="grid" aria-label="Artículos relacionados">
          <article class="card">
            <h3>Contexto nacional y mundial</h3>
            <p>La ludopatía afecta entre 1% y 3% de la población en México; la digitalización ha ampliado el acceso y la vulnerabilidad de jóvenes universitarios.</p>
            <p><a href="#contexto">Leer más</a></p>
          </article>

          <article class="card">
            <h3>Factores de riesgo en Culiacán</h3>
            <p>Familiares, sociales, económicos y psicológicos se combinan para crear un terreno fértil para la adicción.</p>
            <p><a href="#factores">Leer más</a></p>
          </article>

          <article class="card">
            <h3>Delincuencia y lavado de dinero</h3>
            <p>La UIF ha detectado casinos vinculados con operaciones financieras irregulares; la falta de supervisión facilita el blanqueo.</p>
            <p><a href="#lavado">Leer más</a></p>
          </article>

          <article class="card">
            <h3>Testimonios</h3>
            <p>Relatos de Jugadores Anónimos y exjugadores muestran el impacto humano: endeudamiento, pérdida de empleo y riesgo vital.</p>
            <p><a href="#testimonios">Leer más</a></p>
          </article>
        </div>

        <!-- Reportaje completo (secciones) -->
        <article id="reportaje-completo" class="card" style="margin-top:1rem">
          <h2 style="margin-top:0">Reportaje de Investigación</h2>

          <h3 id="contexto">Contexto mundial y nacional</h3>
          <p>La ludopatía es un problema global que afecta a millones. En México, la expansión de apuestas en línea y la publicidad masiva han incrementado la exposición de jóvenes y adultos.</p>

          <h3 id="factores">Factores de riesgo</h3>
          <ul>
            <li><strong>Familiares</strong>: antecedentes de adicciones y falta de comunicación.</li>
            <li><strong>Sociales</strong>: presión de grupo y normalización del juego.</li>
            <li><strong>Económicos</strong>: búsqueda de ingresos rápidos en contextos de precariedad.</li>
            <li><strong>Psicológicos</strong>: ansiedad, baja autoestima y depresión.</li>
          </ul>

          <h3 id="testimonios">Testimonios destacados</h3>
          <blockquote>
            “La ludopatía es un asesino silencioso que te lleva a la cárcel, a la locura o a la muerte.” — Alexander, Jugadores Anónimos, Culiacán
          </blockquote>
          <p>Otros testimonios muestran procesos de recuperación y estrategias de reinserción social.</p>

          <h3 id="consecuencias">Consecuencias sociales</h3>
          <p>Desintegración familiar, endeudamiento, pérdida de patrimonio, problemas de salud mental y proliferación de casas de apuestas en barrios populares.</p>

          <h3 id="lavado">Delincuencia y lavado de dinero</h3>
          <p>Investigaciones y reportes locales señalan que algunos establecimientos funcionan como fachadas para blanquear capitales. La opacidad en permisos y la falta de auditorías facilitan operaciones irregulares.</p>

          <h3 id="complicidad">Complicidad institucional y vacíos legales</h3>
          <p>Permisos ambiguos, tolerancia local y vacíos regulatorios en plataformas digitales son factores que requieren transparencia y reformas.</p>

          <h3 id="conclusiones">Conclusiones y propuestas</h3>
          <ol>
            <li>Campañas de prevención dirigidas a adolescentes y jóvenes.</li>
            <li>Regulación estricta de casinos y plataformas digitales con auditorías públicas.</li>
            <li>Programas de rehabilitación accesibles y gratuitos.</li>
            <li>Transparencia en el otorgamiento de licencias y controles AML robustos.</li>
          </ol>

          <h3 id="referencias">Referencias</h3>
          <p class="meta">Viva la Noticia; El Sol de Sinaloa; Ríodoce; Condusef; UNAM; UIF; CIJ Culiacán.</p>
        </article>

        <section class="card" style="margin-top:1rem">
          <h3>Datos clave</h3>
          <table aria-label="Tabla de cifras">
            <thead>
              <tr><th>Indicador</th><th>Valor</th></tr>
            </thead>
            <tbody>
              <tr><td>Prevalencia estimada en México</td><td>1%–3%</td></tr>
              <tr><td>Pacientes atendidos en Sinaloa (reportes locales)</td><td>120+</td></tr>
              <tr><td>Mercado apuestas deportivas</td><td>50 mil millones MXN anuales (estimado)</td></tr>
              <tr><td>Casinos vinculados detectados por UIF</td><td>13 (a nivel nacional)</td></tr>
            </tbody>
          </table>
        </section>
      </section>

      <aside>
        <div class="side-card" aria-labelledby="sidebar-1">
          <h4 id="sidebar-1">Recuadro práctico</h4>
          <div class="small-list">
            <div><strong>Señales</strong>: priorizar apuestas; mentir; pedir prestado; aislamiento.</div>
            <div><strong>Qué hacer</strong>: detener depósitos; conservar comprobantes; buscar ayuda profesional.</div>
            <a href="#conclusiones">Ver propuestas</a>
          </div>
        </div>

        <div class="side-card" aria-labelledby="sidebar-2">
          <h4 id="sidebar-2">Testimonios breves</h4>
          <div class="small-list">
            <a href="#testimonios">Alexander — Jugadores Anónimos</a>
            <a href="#testimonios">Manuel Velázquez — CIJ Culiacán</a>
            <a href="#testimonios">Historias de recuperación</a>
          </div>
        </div>

        <div class="side-card" aria-labelledby="sidebar-3">
          <h4 id="sidebar-3">Solicitudes de información</h4>
          <p class="meta">Carpetas de investigación, actas de aseguramiento, historial de permisos y borrador de reforma a la Ley de Juegos y Sorteos (pendiente de publicación).</p>
        </div>
      </aside>
    </main>

    <footer>
      <div style="display:flex;justify-content:space-between;align-items:center;gap:1rem;flex-wrap:wrap">
        <div>
          <div style="font-weight:700">Café Expresso Portal</div>
          <div class="meta">Investigación a cargo del equipo de Café Expresso Portal · Miguel Alfredo Miranda Félix · Enero 2026</div>
        </div>
        <div class="meta">Referencias y documentos solicitados serán publicados cuando estén verificados.</div>
      </div>
    </footer>
  </div>

  <script>
    (function(){
      const track = document.querySelector('.carousel-track');
      const prev = document.querySelector('.carousel-btn.prev');
      const next = document.querySelector('.carousel-btn.next');
      if (!track || !prev || !next) return;

      let index = 0;
      const slides = Array.from(track.children);
      function slideWidth() {
        return slides[0]?.getBoundingClientRect().width || 260;
      }
      function maxIndex() {
        const visible = Math.floor(track.parentElement.clientWidth / slideWidth());
        return Math.max(0, slides.length - visible);
      }

      function update() {
        const w = slideWidth();
        const gap = 12;
        const x = -index * (w + gap);
        track.style.transform = `translateX(${x}px)`;
      }

      prev.addEventListener('click', () => {
        index = Math.max(0, index - 1);
        update();
      });

      next.addEventListener('click', () => {
        index = Math.min(maxIndex(), index + 1);
        update();
      });

      window.addEventListener('resize', () => {
        index = Math.min(index, maxIndex());
        update();
      });
    })();
  </script>
</body>
</html>





