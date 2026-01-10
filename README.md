<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>La ludopatía en Culiacán — Especial</title>

  <!-- Google Fonts: Playfair Display (titulares) + Inter (cuerpo) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;800&family=Playfair+Display:wght@700;900&display=swap" rel="stylesheet">

  <style>
    :root{
      --max-width:1100px;
      --accent:#c0392b;
      --muted:#6b7280;
      --serif: "Playfair Display", Georgia, serif;
      --sans: "Inter", Arial, sans-serif;
      --bg:#ffffff;
      --text:#111111;
      --gutter:22px;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:var(--bg);
      color:var(--text);
      font-family:var(--sans);
      /* Base font increased by ~4 points (from 18px to 22px) as requested */
      font-size:22px;
      line-height:1.65;
      font-weight:700;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{max-width:var(--max-width);margin:28px auto;padding:24px}

    header{border-bottom:1px solid #e9e9e9;padding-bottom:18px;margin-bottom:18px}
    /* H1 increased by ~4px equivalent via rem scaling (rem now 22px) */
    h1{
      font-family:var(--serif);
      font-size:3rem; /* larger headline (approx 66px at 22px base) */
      line-height:1.02;
      margin:0 0 8px;
      font-weight:900;
      color:var(--text);
    }
    .byline{color:var(--muted);font-size:18px;margin-bottom:8px;font-weight:700}
    .deck{
      font-family:var(--sans);
      font-size:1.625rem; /* increased ~4 points relative to previous scale */
      font-weight:800;
      color:#222;
      margin:12px 0 14px;
    }
    /* Main lead (texto principal) made noticeably larger */
    .lead{
      background:#f7f7f8;
      padding:18px;
      border-left:6px solid var(--accent);
      margin-bottom:18px;
      font-size:1.5rem; /* larger lead for main text emphasis */
      font-weight:800;
    }

    .grid{display:grid;grid-template-columns:1fr 380px;gap:var(--gutter)}
    @media (max-width:1000px){ .grid{grid-template-columns:1fr} }

    main.article{padding-right:6px}
    aside.sidebar{background:#fbfbfb;padding:16px;border:1px solid #eee;border-radius:6px;font-size:18px;color:var(--muted);font-weight:700}

    /* COVER: use <picture> with provided filenames */
    .cover-wrap{width:100%;overflow:hidden;border-radius:4px;margin:0 0 14px;background:#efefef;position:relative}
    .cover-img{display:block;width:100%;height:68vh; /* slightly taller hero */ object-fit:cover;object-position:center;border-radius:4px}
    .img-fallback{display:none;width:100%;height:68vh;border-radius:4px;background:#ddd;color:#444;display:flex;align-items:center;justify-content:center;font-weight:700;font-size:1.25rem}

    .lead-hero{width:100%;height:48vh;object-fit:cover;object-position:center;border-radius:4px;margin:12px 0}
    .interior-large{width:100%;height:460px;object-fit:cover;object-position:center;border-radius:4px;margin:12px 0}

    .thumb-row{display:flex;gap:10px;margin:12px 0}
    .thumb-row img{width:calc(33.333% - 6.66px);height:160px;object-fit:cover;border-radius:4px}

    h2{
      font-family:var(--serif);
      font-size:1.875rem; /* increased section headings */
      line-height:1.18;
      margin:22px 0 8px;
      font-weight:900;
    }
    h3{
      font-family:var(--sans);
      font-size:1.375rem; /* increased subheadings */
      margin:14px 0 6px;
      font-weight:800;
    }

    p{margin:0 0 1.15rem; font-weight:700; font-size:1.0625rem} /* body paragraphs slightly larger than base */
    ul{margin:0 0 1rem 1.25rem}
    li{margin:0.45rem 0}

    .kpi{display:flex;gap:12px;margin:12px 0 18px}
    .kpi div{background:#fafafa;padding:16px;border:1px solid #eee;border-radius:6px;flex:1;text-align:center}
    .kpi strong{display:block;font-size:24px;color:var(--accent);font-weight:900}

    .quote{font-style:italic;border-left:4px solid #ddd;padding-left:14px;color:#333;margin:12px 0;font-weight:800;font-size:1.125rem}

    .recuadro{background:#fff8f8;border-left:6px solid var(--accent);padding:16px;margin:12px 0;font-weight:800;font-size:1.0625rem}

    table{width:100%;border-collapse:collapse;margin:12px 0;font-size:18px}
    th,td{border:1px solid #e9e9e9;padding:12px;text-align:left}
    th{background:#fafafa;font-weight:800}

    .small{font-size:1rem;color:var(--muted);font-weight:700}
    .credits{font-size:16px;color:var(--muted);margin-top:8px;font-weight:700}
    footer{border-top:1px solid #e6e6e6;padding-top:14px;margin-top:22px;color:var(--muted);font-size:16px;font-weight:700}

    .img-fallback.show{display:flex}

    @media print {
      body{background:#fff;color:#000;font-weight:700}
      .container{max-width:100%;padding:0;margin:0}
      @page { margin:3mm; }
      .cover-wrap{width:100vw;margin:0;overflow:visible}
      .cover-img{width:100%;height:auto;max-height:320mm;object-fit:cover}
      .lead-hero,.interior-large{height:auto;max-height:160mm;page-break-inside:avoid}
      .grid{display:block}
      aside.sidebar{border:none;padding:6mm}
    }

    @media (max-width:900px) {
      .cover-img{height:56vh}
      .lead-hero{height:40vh}
      .interior-large{height:320px}
      .thumb-row img{height:120px}
      body{font-size:20px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>La ludopatía en Culiacán: una adicción que devora hogares y alimenta circuitos opacos</h1>
      <div class="byline"><strong>Autor:</strong> Miguel Alfredo Miranda Félix — <strong>Equipo:</strong> Café Expresso Portal</div>
      <div class="deck">La proliferación de minicasinos y plataformas digitales ha convertido el ocio en una trampa: jóvenes endeudados, familias fracturadas y locales que, según investigaciones, funcionan como fachadas para movimientos financieros irregulares.</div>
      <div class="lead">
        <strong>Culiacán, 2025.</strong> Lo que comenzó como entretenimiento se ha transformado en dependencia: maquinitas en las calles, apps en los bolsillos y una red de vacíos regulatorios que facilita tanto la adicción como el uso de salas de juego para operaciones financieras opacas.
      </div>
      <div class="credits">
        <span><strong>Colaboración:</strong> Centro de Integración Juvenil Culiacán; Jugadores Anónimos; fuentes documentales locales.</span>
      </div>
    </header>

    <div class="grid">
      <main class="article" role="main">
        <!-- COVER: use the exact filenames you uploaded -->
        <div class="cover-wrap" aria-hidden="false">
          <picture>
            <source srcset="apuestas.jpg" type="image/jpeg">
            <img class="cover-img" src="apuestas.jpg" alt="Joven frente a una máquina de apuestas en Culiacán"
                 onerror="this.style.display='none'; this.parentElement.querySelector('.img-fallback').classList.add('show');">
          </picture>
          <div class="img-fallback" aria-hidden="true">Imagen de portada no disponible — apuestas.jpg</div>
        </div>

        <figcaption class="small" style="margin-bottom:12px">
          <strong>Pie:</strong> Culiacán, 2025. Un joven frente a una maquinaría de apuestas en un local de la colonia X; la accesibilidad y la publicidad normalizan el juego entre adolescentes y adultos jóvenes. <span class="small">Foto: Archivo Café Expresso Portal / [Nombre del fotógrafo]</span>
        </figcaption>

        <!-- Lead hero using the uploaded file names -->
        <picture>
          <source srcset="image-48.webp" type="image/webp">
          <img class="lead-hero" src="image-48.webp" alt="Imagen secundaria" 
               onerror="this.style.display='none'; this.insertAdjacentHTML('afterend','<div class=&quot;img-fallback show&quot;>Imagen no disponible — image-48.webp</div>');">
        </picture>

        <h2>Contexto y magnitud</h2>
        <p>La digitalización del juego y la expansión de locales físicos han reducido las barreras de acceso al azar. Apuestas deportivas, microtransacciones y aplicaciones móviles permiten apostar desde cualquier lugar; en paralelo, minicasinos y maquinitas proliferan en colonias populares. En México se estima que entre el <strong>1% y el 3%</strong> de la población padece ludopatía; en Culiacán los centros de atención registran un aumento de consultas, especialmente entre adolescentes y jóvenes.</p>

        <div class="kpi" aria-hidden="true">
          <div><strong>1–3%</strong><span class="small">Prevalencia estimada en México</span></div>
          <div><strong>18–25</strong><span class="small">Grupo más vulnerable (años)</span></div>
          <div><strong>50,000 M</strong><span class="small">Valor aproximado del mercado de apuestas en pesos</span></div>
        </div>

        <h2>Testimonios y trayectorias</h2>
        <p class="quote">“La ludopatía es un asesino silencioso que te lleva a la cárcel, a la locura o a la muerte.” — Alexander, Jugadores Anónimos Culiacán</p>
        <p>Los testimonios recogidos describen una progresión típica: inicio recreativo, aumento de frecuencia y montos, endeudamiento con créditos rápidos, ocultamiento familiar y deterioro laboral y emocional. Muchos afectados relatan que la adicción se instala con rapidez cuando confluyen factores personales y sociales.</p>

        <!-- Use the exact uploaded filenames (double-extension names included as provided) -->
        <picture>
          <source srcset="imagen2.webp.png" type="image/png">
          <img class="interior-large" src="imagen2.webp.png" alt="Imagen 2"
               onerror="this.style.display='none'; this.insertAdjacentHTML('afterend','<div class=&quot;img-fallback show&quot;>Imagen no disponible — imagen2.webp.png</div>');">
        </picture>

        <h2>Factores de riesgo y consecuencias sociales</h2>
        <h3>Factores</h3>
        <ul>
          <li><strong>Familiares:</strong> antecedentes de adicciones, violencia o falta de comunicación.</li>
          <li><strong>Sociales:</strong> presión de grupo y normalización del juego en espacios públicos y digitales.</li>
          <li><strong>Económicos:</strong> búsqueda de ingresos rápidos en contextos de precariedad.</li>
          <li><strong>Psicológicos:</strong> baja autoestima, ansiedad y depresión.</li>
        </ul>

        <h3>Consecuencias</h3>
        <ul>
          <li>Desintegración familiar: discusiones, rupturas y violencia doméstica.</li>
          <li>Endeudamiento y pérdida de patrimonio; en casos extremos, delitos para financiar apuestas.</li>
          <li>Impacto en la salud mental: ansiedad, depresión y riesgo de suicidio.</li>
          <li>Erosión de la cohesión comunitaria y percepción de inseguridad.</li>
        </ul>

        <h2>Vínculos financieros y complicidad institucional</h2>
        <p>Operativos y revisiones han detectado irregularidades en permisos y controles de algunos establecimientos. Fuentes locales y reportes periodísticos señalan que ciertos locales funcionan como fachadas para justificar movimientos de capital, lo que facilita el blanqueo de dinero. Permisos ambiguos, falta de auditorías públicas y controles AML inconsistentes alimentan la percepción de tolerancia o corrupción en distintos niveles administrativos.</p>

        <h2>Respuesta institucional y capacidad de atención</h2>
        <p>Servicios de salud y grupos de apoyo existen, pero la oferta es insuficiente frente a la demanda; hay subregistro de casos y ausencia de protocolos uniformes de derivación. La reforma anunciada a la Ley de Juegos y Sorteos promete mayor control, pero faltan detalles públicos sobre plazos, alcance y recursos para prevención y tratamiento.</p>

        <h2>Propuestas y medidas urgentes</h2>
        <h3>Prevención</h3>
        <ul>
          <li>Campañas dirigidas a adolescentes en escuelas y universidades.</li>
          <li>Restricción de publicidad en horarios y espacios juveniles.</li>
        </ul>

        <h3>Regulación y transparencia</h3>
        <ul>
          <li>Límites por defecto en plataformas y mecanismos obligatorios de autoexclusión.</li>
          <li>Auditorías AML públicas y periódicas; publicación de permisos y sanciones.</li>
          <li>Coordinación entre autoridades financieras y fiscales para rastrear movimientos sospechosos.</li>
        </ul>

        <h3>Atención y rehabilitación</h3>
        <ul>
          <li>Ampliar plazas de tratamiento; programas de rehabilitación accesibles y gratuitos.</li>
          <li>Formación de personal de salud en detección temprana y protocolos de derivación.</li>
        </ul>

        <h2>Periodismo y rendición de cuentas</h2>
        <p>El periodismo de investigación debe exigir y publicar carpetas, actas y auditorías; mapear la oferta de juego y cruzarla con indicadores sociales; proteger fuentes vulnerables. Investigar vínculos entre salas de juego y redes delictivas implica riesgos para la prensa; por eso la verificación documental y la protección de informantes son imprescindibles.</p>

        <div class="recuadro">
          <strong>Recuadro práctico</strong>
          <p><strong>Señales de riesgo:</strong> priorizar apuestas; mentir sobre tiempo o dinero; pedir prestado; aislamiento; cambios bruscos de humor; intentos autolesivos.</p>
          <p><strong>Qué hacer ahora:</strong> detener depósitos; conservar comprobantes; bloquear tarjetas vinculadas; hablar con un familiar; buscar apoyo en salud mental o grupos como Jugadores Anónimos; solicitar autoexclusión si está disponible; buscar asesoría legal ante deudas.</p>
        </div>

        <h2>Metodología y ética</h2>
        <p>La investigación combinó revisión de reportes locales, entrevistas con afectados y especialistas, y solicitudes formales de información. Se protegieron identidades de fuentes vulnerables y se evitó presentar como hechos judiciales las indagatorias que aún están en curso; toda referencia a irregularidades financieras se presenta como presunta hasta contar con documentos oficiales.</p>

        <h2>Referencias</h2>
        <ul>
          <li>Viva la Noticia — CIJ alerta sobre ludopatía en adolescentes en Culiacán</li>
          <li>El Sol de Sinaloa — Ludopatía: vicios que cuestan, pero no matan</li>
          <li>Los Noticieristas — Testimonios de Jugadores Anónimos</li>
          <li>Ríodoce — Detectan casinos vinculados con lavado de dinero en Sinaloa</li>
          <li>Meganoticias Culiacán — Plataformas digitales de apuestas bajo investigación de la UIF</li>
          <li>UNAM Global — El juego patológico como problema de salud pública en México</li>
          <li>Condusef — Impacto financiero de las apuestas en jóvenes mexicanos</li>
        </ul>
      </main>

      <aside class="sidebar" role="complementary" aria-label="Imágenes y metadatos">
        <h3>Imágenes y metadatos</h3>

        <table>
          <thead>
            <tr><th>Nombre en repo</th><th>Uso sugerido</th><th>Ruta exacta</th></tr>
          </thead>
          <tbody>
            <tr><td>apuestas.jpg</td><td>Portada principal</td><td>apuestas.jpg</td></tr>
            EADME.md
Enhance styles and image handling in README
            <tr><td>casino2.jpg</td><td>Imagen secundaria / miniatura</td><td>casino2.jpg</td></tr>
            <tr><td>casino3.webp/td><td>Imagen interior (renombrar recomendado)</td><td>casino3.webp/td></tr>
            <tr><td>casino4.png</td><td>Imagen interior (renombrar recommended)</td><td>casino4.png</td></tr>
            <tr><td>casino5.png</td><td>Imagen interior (renombrar recommended)</td><td>casino5.png</td></tr>
            <tr><td>casino6.jpg</td><td>Imagen interior (renombrar recommended)</td><td>casino6.jpg</td></tr>
            
          </tbody>
        </table>

        <h3>Especificaciones técnicas</h3>
        <ul class="small">
          <li>Verifica que los archivos existan con exactamente esos nombres en la misma carpeta que este HTML.</li>
          <li>Si renombraste archivos, actualiza las rutas en el HTML para que coincidan exactamente (mayúsculas/minúsculas incluidas).</li>
          <li>Para mejor compatibilidad, considera renombrar los archivos con doble extensión a una sola extensión real (por ejemplo, imagen2.png).</li>
        </ul>

        <h3>Checklist antes de publicar</h3>
        <ol class="small">
          <li>Confirma que <code>apuestas.jpg</code> esté presente y accesible.</li>
          <li>Si alguna imagen no carga, revisa la consola del navegador (F12 → Network) para ver errores 404 y ajustar nombres.</li>
          <li>Reemplaza <code>[Nombre del fotógrafo]</code> por el crédito real antes de publicar.</li>
        </ol>
      </aside>
    </div>

    <footer>
      <div class="small">
        <strong>Pie de redacción:</strong> Investigación a cargo del equipo de Café Expresso Portal. Para enviar testimonios, documentos o denuncias: [correo de redacción — pendiente de confirmación].<br>
        <strong>Nota editorial:</strong> Toda referencia a irregularidades financieras se presenta como presunta hasta contar con documentos oficiales.
      </div>
    </footer>
  </div>

  <script>
    // Comprueba imágenes tras carga y activa fallback si fallan
    document.addEventListener('DOMContentLoaded', function(){
      document.querySelectorAll('img').forEach(function(img){
        if (!img.complete || img.naturalWidth === 0) {
          var parent = img.parentElement;
          var container = parent.closest('.cover-wrap') || parent;
          var fallback = container.querySelector('.img-fallback');
          if (fallback) {
            fallback.classList.add('show');
            img.style.display = 'none';
          } else {
            var fb = document.createElement('div');
            fb.className = 'img-fallback show';
            fb.textContent = 'Imagen no disponible — ' + (img.getAttribute('src') || 'sin ruta');
            img.insertAdjacentElement('afterend', fb);
            img.style.display = 'none';
          }
        }
      });
    });
  </script>
</body>
</html>



