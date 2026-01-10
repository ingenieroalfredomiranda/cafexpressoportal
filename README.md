<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>La ludopatía en Culiacán — Especial</title>

  <!-- Google Fonts: Playfair Display (titulares) + Inter (cuerpo) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">

  <style>
    /*
      Tipografía y escala pensadas para reproducir el aspecto sobrio y legible
      de un diario de calidad. Ajustes de imagen pensados para web y para impresión:
      - Portada: imagen a página completa (full-bleed) en pantalla y en impresión.
      - Imágenes interiores: tamaños fijos relativos a la columna y a la doble página.
      - Sidebar: imágenes verticales con ancho fijo.
    */

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

    /* Reset / base */
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:var(--bg);
      color:var(--text);
      font-family:var(--sans);
      font-size:16px;
      line-height:1.6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      max-width:var(--max-width);
      margin:28px auto;
      padding:24px;
    }

    /* Header / masthead */
    header{border-bottom:1px solid #e9e9e9;padding-bottom:18px;margin-bottom:18px}
    h1{
      font-family:var(--serif);
      font-size:2.25rem; /* ≈36px */
      line-height:1.05;
      margin:0 0 6px;
      font-weight:700;
      color:var(--text);
    }
    .byline{color:var(--muted);font-size:14px;margin-bottom:8px}
    .deck{
      font-family:var(--sans);
      font-size:1.125rem; /* ≈18px */
      font-weight:600;
      color:#222;
      margin:12px 0 14px;
    }
    .lead{
      background:#f7f7f8;
      padding:14px;
      border-left:4px solid var(--accent);
      margin-bottom:18px;
      font-size:1rem; /* ≈16px */
      font-weight:500;
    }

    /* Layout */
    .grid{display:grid;grid-template-columns:1fr 360px;gap:var(--gutter)}
    @media (max-width:900px){ .grid{grid-template-columns:1fr} }

    main.article{padding-right:6px}
    aside.sidebar{
      background:#fbfbfb;padding:14px;border:1px solid #eee;border-radius:6px;
      font-size:14px;color:var(--muted);
    }

    /* IMAGE SIZING RULES (web) */
    /* Portada: full-bleed look on screen: wide, tall, with focal crop */
    .cover-wrap{
      width:100%;
      overflow:hidden;
      border-radius:4px;
      margin:0 0 14px;
    }
    .cover-img{
      display:block;
      width:100%;
      height:60vh;               /* tall, newspaper-like hero */
      object-fit:cover;          /* crop to focal point */
      object-position:center;
      border-radius:4px;
    }

    /* Lead / double-page hero for interior (large image) */
    .lead-hero{
      width:100%;
      height:42vh;               /* large interior hero */
      object-fit:cover;
      object-position:center;
      border-radius:4px;
      margin:12px 0;
    }

    /* Standard large interior image (single column) */
    .interior-large{
      width:100%;
      height:360px;
      object-fit:cover;
      object-position:center;
      border-radius:4px;
      margin:12px 0;
    }

    /* Sidebar images (vertical) */
    .sidebar img{
      width:100%;
      height:auto;
      border-radius:4px;
      display:block;
      margin-bottom:12px;
    }

    /* Small inline thumbnails */
    .thumb-row{display:flex;gap:10px;margin:12px 0}
    .thumb-row img{width:calc(33.333% - 6.66px);height:120px;object-fit:cover;border-radius:4px}

    /* Headings inside article */
    h2{
      font-family:var(--serif);
      font-size:1.25rem; /* ≈20px */
      line-height:1.25;
      margin:22px 0 8px;
      font-weight:600;
    }
    h3{
      font-family:var(--sans);
      font-size:1rem; /* ≈16px */
      margin:14px 0 6px;
      font-weight:600;
    }

    p{margin:0 0 1rem}
    ul{margin:0 0 1rem 1.15rem}
    li{margin:0.35rem 0}

    .kpi{display:flex;gap:12px;margin:12px 0 18px}
    .kpi div{background:#fafafa;padding:12px;border:1px solid #eee;border-radius:6px;flex:1;text-align:center}
    .kpi strong{display:block;font-size:20px;color:var(--accent)}

    .quote{font-style:italic;border-left:3px solid #ddd;padding-left:12px;color:#333;margin:12px 0}

    .recuadro{background:#fff8f8;border-left:4px solid var(--accent);padding:12px;margin:12px 0}

    table{width:100%;border-collapse:collapse;margin:12px 0;font-size:14px}
    th,td{border:1px solid #e9e9e9;padding:8px;text-align:left}
    th{background:#fafafa}

    .small{font-size:0.875rem;color:var(--muted)}
    .credits{font-size:13px;color:var(--muted);margin-top:8px}

    footer{border-top:1px solid #e6e6e6;padding-top:14px;margin-top:22px;color:var(--muted);font-size:13px}

    /* PRINT STYLES: try to preserve the newspaper feel when printing to PDF/press */
    @media print {
      :root { --gutter:10px; }
      body{background:#fff;color:#000}
      .container{max-width:100%;padding:0;margin:0}
      header{page-break-after:avoid;border-bottom:none;padding:0 6mm 6mm}
      /* Make the cover image full-bleed on print: use page margins and scale */
      @page { margin:3mm; }
      .cover-wrap{width:100vw;margin:0;overflow:visible}
      .cover-img{
        width:100%;
        height: auto;
        max-height: 320mm; /* allow tall hero for full-page feel */
        object-fit:cover;
      }
      /* Interior large images: occupy a large portion of the column */
      .lead-hero, .interior-large{
        height:auto;
        max-height:160mm;
        page-break-inside:avoid;
      }
      /* Sidebar becomes a block below article in print */
      .grid{display:block}
      aside.sidebar{border:none;padding:6mm}
      .thumb-row img{height:60px}
      /* Hide interactive-only elements */
      .kpi{display:block}
    }

    /* Responsive adjustments for small screens */
    @media (max-width:900px) {
      .cover-img{height:44vh}
      .lead-hero{height:34vh}
      .interior-large{height:220px}
      .thumb-row img{height:90px}
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
        <!-- COVER (hero) -->
        <div class="cover-wrap" aria-hidden="false">
          <!-- Reemplaza src por la ruta real del archivo portada_apuestas.jpg -->
          <img class="cover-img" src="portada_apuestas.jpg" alt="Joven sentado frente a una máquina de apuestas en un local de Culiacán.">
        </div>
        <figcaption class="small" style="margin-bottom:12px">
          <strong>Pie:</strong> Culiacán, 2025. Un joven frente a una maquinaría de apuestas en un local de la colonia X; la accesibilidad y la publicidad normalizan el juego entre adolescentes y adultos jóvenes. <span class="small">Foto: Archivo Café Expresso Portal / [Nombre del fotógrafo]</span>
        </figcaption>

        <!-- Interior lead hero (large image for double-page feel) -->
        <img class="lead-hero" src="maquinitas_calle_comercial.jpg" alt="Maquinitas y puntos de apuestas en una calle comercial de Culiacán.">

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

        <!-- Standard interior large image -->
        <img class="interior-large" src="fachada_minicasino_colonia.jpg" alt="Fachada de un minicasino en una colonia popular de Culiacán.">

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
            <tr><th>Nombre original</th><th>Nombre asignado</th><th>Pie de foto breve</th></tr>
          </thead>
          <tbody>
            <tr><td>apuestas</td><td>portada_apuestas.jpg</td><td>Culiacán, 2025. Un joven frente a una maquinaría de apuestas; la accesibilidad normaliza el juego.</td></tr>
            <tr><td>imagen2.webp</td><td>fachada_minicasino_colonia.jpg</td><td>Fachada de un minicasino en una colonia popular; vecinos denuncian cercanía con escuelas.</td></tr>
            <tr><td>imagen3.webp</td><td>maquinitas_calle_comercial.jpg</td><td>Maquinitas y puntos de apuestas en una calle comercial; la presencia cotidiana facilita el acceso.</td></tr>
            <tr><td>imagen4.webp</td><td>grupo_apoyo_testimonios.jpg</td><td>Grupo de apoyo local donde exjugadores comparten su proceso de recuperación.</td></tr>
            <tr><td>imagen5</td><td>documentos_inspecciones_actas.jpg</td><td>Documentos y actas relacionados con inspecciones; la prensa exige transparencia.</td></tr>
            <tr><td>imagen5.webp</td><td>pantalla_app_apuestas.jpg</td><td>Pantalla de teléfono con una app de apuestas deportivas; la digitalización facilita el acceso.</td></tr>
          </tbody>
        </table>

        <h3>Especificaciones técnicas</h3>
        <ul class="small">
          <li>Portada (web): hero full-bleed, altura recomendada 60vh; formato JPG/PNG sRGB; ancho mínimo 1600 px para buena calidad en pantallas grandes.</li>
          <li>Portada (impresión): imagen en alta resolución (300 dpi) y formato TIFF/JPG; preparar versión con sangrado 3 mm.</li>
          <li>Imágenes interiores grandes: 1200–1600 px ancho (web); 200–300 dpi (impresión).</li>
          <li>Sidebar / verticals: 900–1100 px alto (web) o 200–250 dpi (impresión).</li>
          <li>Accesibilidad: incluir atributo alt y descripciones largas en la ficha de la imagen.</li>
          <li>Protección de identidades: difuminar rostros si las fuentes lo solicitan.</li>
        </ul>

        <h3>Checklist antes de publicar</h3>
        <ol class="small">
          <li>Reemplazar [Nombre del fotógrafo] por créditos reales.</li>
          <li>Verificar permisos de publicación y consentimiento de fuentes.</li>
          <li>Confirmar resolución y perfiles de color de todas las imágenes.</li>
          <li>Marcar como presuntas las irregularidades hasta contar con documentos oficiales.</li>
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
</body>
</html>






