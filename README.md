<!-- Hero -->
<section class="hero" aria-labelledby="main-headline">
  <article class="hero-main">
    <div class="kicker">Investigación</div> 
    <h1 id="main-headline" class="headline">
      La ludopatía en Culiacán: una adicción silenciosa que devora vidas y dinero
    </h1>

    <div class="byline">
      Por <strong>Café Expreso Portal</strong> — Investigación y reportaje
    </div>

    <p class="summary" style="color:var(--muted);font-size:13.5px;margin-top:6px;">
      Resumen: Este reportaje documenta factores de riesgo, trayectorias clínicas, impacto económico y vínculos con lavado de dinero en Sinaloa. Incluye testimonios, solicitudes de información y propuestas de política pública.
    </p>

    <!-- Portada principal -->
    <figure class="hero-image" style="position:relative;">
      <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/apuestas.jpg"
           alt="Portada principal: apuestas en Culiacán"
           class="imagen-ajustada responsive-img"
           loading="lazy"
           style="width:100%;height:auto;display:block;object-fit:cover;max-width:100%;border-radius:6px;" />
      <figcaption class="hero-caption"
                  style="position:absolute;bottom:0;left:0;width:100%;
                         background:rgba(0,0,0,0.7);color:#fff;padding:16px;
                         text-align:center;border-radius:0 0 6px 6px;">
        <div style="font-size:22px;font-weight:bold;color:#ff5252;margin-bottom:8px;">
          La apuesta perdida — Culiacán en la ruina del juego
        </div>
      </figcaption>
    </figure>
  </article>
</section>

<!-- Bloque: imagen de ayuda + botón para abrir el cuestionario -->
<section aria-label="Captura principal">
  <figure class="capture-test" aria-labelledby="captureTitle">
    <img src="https://ingenieroalfredomiranda.github.io/cafexpressoportal/ayuda.jpg"
         alt="Cómo ayudar: campañas de prevención, regulación y programas de rehabilitación"
         loading="lazy"
         class="imagen-ajustada responsive-img" />
    <figcaption id="captureTitle" class="capture-caption">
      <strong>Cómo ayudar</strong><br />
      Se proponen campañas de prevención, regulación estricta de plataformas digitales,
      programas de rehabilitación accesibles y transparencia en licencias.
      <br />
      <button id="openQuiz" class="btn-access-test" aria-haspopup="dialog" aria-controls="quizModal">
        Acceder al test
      </button>
    </figcaption>
  </figure>
</section>

<script>
(function(){
  // --- Smooth scroll + foco accesible para anclas internas
  document.querySelectorAll('a[href^="#"]').forEach(a=>{
    a.addEventListener('click', function(e){
      const href = this.getAttribute('href');
      if(href === '#quizModal'){ /* handled by modal opener below */ return; }
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

  // --- Modal open/close
  const modal = document.getElementById('quizModal');
  const openFromCapture = document.querySelector('.btn-access-test');
  const openButtons = document.querySelectorAll('.quiz-open');
  const closeButtons = modal ? modal.querySelectorAll('.quiz-close, #quizCloseFooter, .quiz-backdrop') : [];

  function openModal(){
    if(!modal) return;
    modal.hidden = false;
    document.body.style.overflow = 'hidden';
    setTimeout(()=> {
      const first = modal.querySelector('input[type="radio"]');
      if(first) first.focus();
      else modal.querySelector('.quiz-close')?.focus();
    }, 120);
  }
  function closeModal(){
    if(!modal) return;
    modal.hidden = true;
    document.body.style.overflow = '';
    const last = document.querySelector('.btn-access-test, .quiz-open');
    if(last) last.focus();
  }

  openFromCapture?.addEventListener('click', e=>{ e.preventDefault(); openModal(); });
  openButtons.forEach(btn => btn.addEventListener('click', e=>{ e.preventDefault(); openModal(); }));
  closeButtons.forEach(el=> el.addEventListener('click', ()=> closeModal()));
  document.addEventListener('keydown', e=>{
    if(e.key === 'Escape' && modal && !modal.hidden) closeModal();
  });

  // --- Cuestionario: preguntas, render y evaluación
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

  const thresholds = {
    riesgoBajo: 0,   // 0 respuestas afirmativas
    riesgoMedio: 2,  // 2–3 respuestas afirmativas
    riesgoAlto: 4    // 4 o más respuestas afirmativas
  };

  const quizList = document.getElement
