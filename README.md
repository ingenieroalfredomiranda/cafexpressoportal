<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Galería — Café Expresso Portal</title>
  <style>
    :root{
      --accent:#c62828;
      --muted:#666;
      --bg:#fafafa;
      --card:#ffffff;
      --maxw:1200px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    html,body{height:100%}
    body{margin:0;background:var(--bg);color:#111;line-height:1.5}
    .container{max-width:var(--maxw);margin:24px auto;padding:20px}
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
    @media (max-width:1000px){
      .gallery{grid-template-columns:repeat(2,1fr)}
      .group-row picture img{height:180px}
    }
    @media (max-width:600px){
      .gallery{grid-template-columns:1fr}
      .group-row{flex-direction:column}
      .group-row picture img{height:220px}
    }

    /* Modal ligero (visibilidad controlada por clase .open) */
    .modal{
      position:fixed;inset:0;display:flex;align-items:center;justify-content:center;padding:20px;z-index:9999;
      background:rgba(0,0,0,0.85);
      visibility:hidden;opacity:0;pointer-events:none;transition:opacity .18s ease, visibility .18s;
    }
    .modal.open{visibility:visible;opacity:1;pointer-events:auto}
    .modal-content{max-width:1100px;width:100%;display:flex;flex-direction:column;align-items:center;gap:12px;position:relative}
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
    </header>

    <main class="card" role="main" aria-labelledby="galeria-title">
      <h2 id="galeria-title" style="margin-top:0">Galería: evidencia visual</h2>

      <div class="gallery" role="list" aria-label="Galería de imágenes">

        <!-- imagen1: apuestas -->
        <figure class="gallery-item single-item" role="listitem" aria-labelledby="cap-apuestas">
          <picture>
            <source type="image/webp" srcset="images/apuestas-sm.webp 600w, images/apuestas-md.webp 1200w, images/apuestas-lg.webp 2000w" sizes="(max-width:600px) 100vw, (max-width:1200px) 50vw, 33vw">
            <img class="img-apuestas" src="images/apuestas-md.webp" alt="Letrero de casino con la palabra APUESTAS" loading="lazy" width="1200" height="800" decoding="async">
          </picture>
          <figcaption id="cap-apuestas"><span class="caption-strong">Apuestas</span> — Fachada y letrero; descripción en el pie de foto.</figcaption>
        </figure>

        <!-- imagen2: testimonio anónimo -->
        <figure class="gallery-item single-item" role="listitem" aria-labelledby="cap-testimonio">
          <picture>
            <source type="image/webp" srcset="images/imagen2-sm.webp 600w, images/imagen2-md.webp 1200w, images/imagen2-lg.webp 2000w" sizes="(max-width:600px) 100vw, (max-width:1200px) 50vw, 33vw">
            <img src="images/imagen2-md.webp" alt="Persona anónima frente a letrero de casino" loading="lazy" width="1200" height="800" decoding="async">
          </picture>
          <figcaption id="cap-testimonio">Testimonio anónimo — fachada de casino; advertencia de contenido sensible.</figcaption>
        </figure>

        <!-- imagen3 + imagen31 -->
        <figure class="gallery-item grouped" role="listitem" aria-labelledby="cap-maquinas">
          <div class="group-title">Máquinas y salas</div>
          <div class="group-row" role="group" aria-label="Máquinas imagen3 e imagen31">
            <picture>
              <source type="image/webp" srcset="images/imagen3-sm.webp 600w, images/imagen3-md.webp 1200w, images/imagen3-lg.webp 2000w">
              <img src="images/imagen3-md.webp" alt="Máquinas tragamonedas interior" loading="lazy" width="800" height="533" decoding="async">
            </picture>
            <picture>
              <source type="image/webp" srcset="images/imagen31-sm.webp 600w, images/imagen31-md.webp 1200w, images/imagen31-lg.webp 2000w">
              <img src="images/imagen31-md.webp" alt="Máquinas tragamonedas interior" loading="lazy" width="800" height="533" decoding="async">
            </picture>
          </div>
          <figcaption id="cap-maquinas">Máquinas y ambiente de juego — pie de foto descriptivo.</figcaption>
        </figure>

        <!-- imagen4 + imagen41 -->
        <figure class="gallery-item grouped small" role="listitem" aria-labelledby="cap-operativos">
          <div class="group-title">Operativos y mesas (versión compacta)</div>
          <div class="group-row small-row" role="group" aria-label="Operativos imagen4 e imagen41">
            <picture>
              <source type="image/webp" srcset="images/imagen4-sm.webp 400w, images/imagen4-md.webp 800w">
              <img src="images/imagen4-md.webp" alt="Mesa y elementos de apuestas" loading="lazy" width="600" height="400" decoding="async">
            </picture>
            <picture>
              <source type="image/webp" srcset="images/imagen41-sm.webp 400w, images/imagen41-md.webp 800w">
              <img src="images/imagen41-md.webp" alt="Máquinas y mesa" loading="lazy" width="600" height="400" decoding="async">
            </picture>
          </div>
          <figcaption id="cap-operativos">Operativos y evidencia simbólica — versión compacta.</figcaption>
        </figure>

      </div>
    </main>
  </div>

  <!-- Modal accesible -->
  <div id="img-modal" class="modal" role="dialog" aria-modal="true" aria-hidden="true" aria-label="Visor de imagen">
    <div class="modal-content" role="document">
      <button class="close" id="modal-close" aria-label="Cerrar imagen">Cerrar</button>
      <img id="modal-img" src="" alt="">
      <div id="modal-caption" class="caption" aria-live="polite"></div>
    </div>
  </div>

  <script>
    (function () {
      const gallery = document.querySelector('.gallery');
      const modal = document.getElementById('img-modal');
      const modalImg = document.getElementById('modal-img');
      const modalCaption = document.getElementById('modal-caption');
      const closeBtn = document.getElementById('modal-close');
      let lastFocused = null;
      let focusableElements = [];
      let firstFocusable = null;
      let lastFocusable = null;

      // Delegated click: abre modal al hacer clic en una imagen dentro de la galería
      document.addEventListener('click', (e) => {
        // si el click fue dentro del modal, no procesar aquí
        if (e.target.closest('#img-modal')) return;
        const img = e.target.closest('img');
        if (!img) return;
        if (!gallery.contains(img)) return;
        openModal(img);
      });

      function openModal(imgElement) {
        lastFocused = document.activeElement;
        // usa currentSrc para respetar srcset; fallback a src
        modalImg.src = imgElement.currentSrc || imgElement.src || '';
        modalImg.alt = imgElement.alt || '';
        modalCaption.textContent = imgElement.alt || '';
        modal.classList.add('open');
        modal.setAttribute('aria-hidden', 'false');
        document.body.style.overflow = 'hidden';
        // preparar trampa de foco
        setupFocusTrap();
        // enfocar el botón cerrar
        closeBtn.focus();
      }

      function closeModal() {
        modal.classList.remove('open');
        modal.setAttribute('aria-hidden', 'true');
        document.body.style.overflow = '';
        // limpiar src para liberar memoria
        modalImg.src = '';
        modalImg.alt = '';
        modalCaption.textContent = '';
        // restaurar foco
        if (lastFocused && typeof lastFocused.focus === 'function') {
          lastFocused.focus();
        }
      }

      // Cerrar con Escape
      document.addEventListener('keydown', (e) => {
        if (e.key === 'Escape' && modal.classList.contains('open')) {
          e.preventDefault();
          closeModal();
        }
        if (e.key === 'Tab' && modal.classList.contains('open')) {
          handleTabKey(e);
        }
      });

      // Cerrar al hacer clic fuera del contenido (overlay)
      modal.addEventListener('click', (e) => {
        if (e.target === modal) closeModal();
      });

      closeBtn.addEventListener('click', closeModal);

      // Configura elementos enfocables dentro del modal para trampa de foco
      function setupFocusTrap() {
        focusableElements = modal.querySelectorAll('button, [href], input, select, textarea, [tabindex]:not([tabindex="-1"])');
        focusableElements = Array.prototype.slice.call(focusableElements);
        firstFocusable = focusableElements[0] || closeBtn;
        lastFocusable = focusableElements[focusableElements.length - 1] || closeBtn;
      }

      function handleTabKey(e) {
        if (focusableElements.length === 0) {
          e.preventDefault();
          return;
        }
        const active = document.activeElement;
        if (e.shiftKey) {
          if (active === firstFocusable) {
            e.preventDefault();
            lastFocusable.focus();
          }
        } else {
          if (active === lastFocusable) {
            e.preventDefault();
            firstFocusable.focus();
          }
        }
      }

      // Mejora: si el modal está abierto, evitar que el foco salga (doble chequeo)
      document.addEventListener('focus', function (event) {
        if (!modal.classList.contains('open')) return;
        if (!modal.contains(event.target)) {
          event.stopPropagation();
          firstFocusable.focus();
        }
      }, true);
    })();
  </script>
</body>
</html>



