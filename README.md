<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Galería — Café Expresso Portal</title>
  <meta name="description" content="Galería de imágenes del reportaje sobre ludopatía en Culiacán. Agrupaciones y advertencias sobre menores." />
  <style>
    :root{
      --accent:#c62828;
      --muted:#666;
      --bg:#fafafa;
      --card:#ffffff;
      --maxw:1200px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    html,body{height:100%;}
    body{margin:0;background:var(--bg);color:#111;line-height:1.5}
    .container{max-width:var(--maxw);margin:24px auto;padding:20px;}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px;margin-bottom:12px}
    header h1{font-size:1.1rem;margin:0}
    .card{background:var(--card);padding:16px;border-radius:10px;box-shadow:0 6px 18px rgba(16,24,40,0.04)}
    .gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:16px}
    .gallery-item{background:#fff;border-radius:8px;padding:10px;box-shadow:0 6px 18px rgba(16,24,40,0.04);overflow:hidden}
    .gallery-item img{width:100%;height:auto;display:block;border-radius:6px;object-fit:cover}
    .gallery-item figcaption{font-size:0.92rem;color:var(--muted);margin-top:8px}
    .grouped .group-title{font-weight:700;margin-bottom:8px}
    .group-row{display:flex;gap:8px}
    .group-row picture{flex:1;display:block}
    .group-row picture img{height:220px;object-fit:cover;border-radius:6px}
    .grouped.small .group-row picture img{height:140px}
    .single-item .img-apuestas{object-fit:cover;object-position:60% 50%;max-height:360px;border-radius:6px}
    .caption-strong{font-weight:700}
    /* Responsive */
    @media (max-width:1000px){.gallery{grid-template-columns:repeat(2,1fr)} .group-row picture img{height:180px}}
    @media (max-width:600px){.gallery{grid-template-columns:1fr}.group-row{flex-direction:column}.group-row picture img{height:220px}}
    /* Modal ligero */
    .modal{position:fixed;inset:0;background:rgba(0,0,0,0.85);display:flex;align-items:center;justify-content:center;padding:20px;z-index:9999;visibility:hidden;opacity:0;transition:opacity .18s}
    .modal.open{visibility:visible;opacity:1}
    .modal-content{max-width:1100px;width:100%;display:flex;flex-direction:column;align-items:center;gap:12px}
    .modal img{max-width:100%;max-height:80vh;border-radius:8px;box-shadow:0 10px 30px rgba(0,0,0,0.6)}
    .modal .close{position:absolute;top:18px;right:18px;background:#fff;border-radius:6px;padding:6px 10px;font-weight:700;cursor:pointer;border:0}
    .modal .caption{color:#fff;text-align:center;max-width:90%;font-size:0.98rem}
    /* Accessibility focus */
    a:focus, button:focus, input:focus {outline:3px solid rgba(198,40,40,0.18);outline-offset:2px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Café Expresso Portal — Galería visual</h1>
      <div class="small" aria-hidden="true">Imágenes agrupadas y advertencias sobre menores</div>
    </header>

    <main class="card" role="main" aria-labelledby="galeria-title">
      <h2 id="galeria-title" style="margin-top:0">Galería: evidencia visual</h2>

      <div class="gallery" role="list">

        <!-- imagen1: apuestas (ajuste para que se vean las letras completas) -->
        <figure class="gallery-item single-item" role="listitem" aria-labelledby="cap-apuestas">
          <picture>
            <source type="image/webp" srcset="images/apuestas-sm.webp 600w, images/apuestas-md.webp 1200w, images/apuestas-lg.webp 2000w" sizes="(max-width:600px) 100vw, (max-width:1200px) 50vw, 33vw">
            <img class="img-apuestas" src="images/apuestas-md.webp" alt="Letrero completo de casino: APUESTAS" loading="lazy" width="1200" height="800">
          </picture>
          <figcaption id="cap-apuestas"><span class="caption-strong">Apuestas</span> — Fachada y letrero; niños también están cayendo en este vicio.</figcaption>
        </figure>

        <!-- imagen2: testimonio anónimo -->
        <figure class="gallery-item single-item" role="listitem" aria-labelledby="cap-testimonio">
          <picture>
            <source type="image/webp" srcset="images/imagen2-sm.webp 600w, images/imagen2-md.webp 1200w, images/imagen2-lg.webp 2000w" sizes="(max-width:600px) 100vw, (max-width:1200px) 50vw, 33vw">
            <img src="images/imagen2-md.webp" alt="Persona anónima frente a letrero de casino" loading="lazy" width="1200" height="800">
          </picture>
          <figcaption id="cap-testimonio">Testimonio anónimo — fachada de casino; advertencia: menores también afectados.</figcaption>
        </figure>

        <!-- imagen3 + imagen31: mismas en un mismo apartado -->
        <figure class="gallery-item grouped" role="listitem" aria-labelledby="cap-maquinas">
          <div class="group-title">Máquinas y salas</div>
          <div class="group-row" role="group" aria-label="Máquinas imagen3 e imagen31">
            <picture>
              <source type="image/webp" srcset="images/imagen3-sm.webp 600w, images/imagen3-md.webp 1200w, images/imagen3-lg.webp 2000w">
              <img src="images/imagen3-md.webp" alt="Máquinas tragamonedas interior (imagen3)" loading="lazy" width="800" height="533">
            </picture>
            <picture>
              <source type="image/webp" srcset="images/imagen31-sm.webp 600w, images/imagen31-md.webp 1200w, images/imagen31-lg.webp 2000w">
              <img src="images/imagen31-md.webp" alt="Máquinas tragamonedas interior (imagen31)" loading="lazy" width="800" height="533">
            </picture>
          </div>
          <figcaption id="cap-maquinas">Máquinas y ambiente de juego — niños y jóvenes también están expuestos a estas salas.</figcaption>
        </figure>

        <!-- imagen4 + imagen41: mini‑galería reducida (tamaño menor) -->
        <figure class="gallery-item grouped small" role="listitem" aria-labelledby="cap-operativos">
          <div class="group-title">Operativos y mesas (versión compacta)</div>
          <div class="group-row small-row" role="group" aria-label="Operativos imagen4 e imagen41">
            <picture>
              <source type="image/webp" srcset="images/imagen4-sm.webp 400w, images/imagen4-md.webp 800w">
              <img src="images/imagen4-md.webp" alt="Mesa y elementos de apuestas (imagen4)" loading="lazy" width="600" height="400">
            </picture>
            <picture>
              <source type="image/webp" srcset="images/imagen41-sm.webp 400w, images/imagen41-md.webp 800w">
              <img src="images/imagen41-md.webp" alt="Máquinas y mesa (imagen41)" loading="lazy" width="600" height="400">
            </picture>
          </div>
          <figcaption id="cap-operativos">Operativos y evidencia simbólica — versión compacta; atención: menores también están cayendo en el vicio.</figcaption>
        </figure>

      </div>
    </main>
  </div>

  <!-- Modal ligero -->
  <div id="img-modal" class="modal" role="dialog" aria-modal="true" aria-hidden="true" style="display:none">
    <div class="modal-content card" role="document">
      <button class="close" aria-label="Cerrar imagen" onclick="closeModal()">X</button>
      <img src="" alt="" id="modal-img">
      <div class="caption" id="modal-caption" aria-live="polite"></div>
    </div>
  </div>

  <script>
    // Delegated click handler to open modal for any image inside .gallery
    document.addEventListener('click', (e) => {
      const img = e.target.closest('.gallery-item img');
      if(img) openModal(img.src, img.alt);
    });

    function openModal(src, alt){
      const modal = document.getElementById('img-modal');
      const modalImg = document.getElementById('modal-img');
      const modalCaption = document.getElementById('modal-caption');
      modalImg.src = src;
      modalImg.alt = alt || '';
      modalCaption.textContent = alt || '';
      modal.style.display = 'flex';
      modal.classList.add('open');
      modal.setAttribute('aria-hidden', 'false');
      document.body.style.overflow = 'hidden';
      // focus management
      const closeBtn = modal.querySelector('.close');
      if(closeBtn) closeBtn.focus();
    }

    function closeModal(){
      const modal = document.getElementById('img-modal');
      if(!modal) return;
      modal.classList.remove('open');
      modal.style.display = 'none';
      modal.setAttribute('aria-hidden', 'true');
      document.body.style.overflow = '';
      // clear src to release memory
      const modalImg = document.getElementById('modal-img');
      if(modalImg) modalImg.src = '';
    }

    // Close modal with Escape key
    document.addEventListener('keydown', (e) => {
      if(e.key === 'Escape'){
        const modal = document.getElementById('img-modal');
        if(modal && modal.classList.contains('open')) closeModal();
      }
    });

    // Improve keyboard accessibility: trap focus inside modal while open
    document.addEventListener('focus', function(event) {
      const modal = document.getElementById('img-modal');
      if(!modal) return;
      if(modal.classList.contains('open') && !modal.contains(event.target)){
        event.stopPropagation();
        modal.querySelector('.close').focus();
      }
    }, true);
  </script>
</body>
</html>


