<!doctype html>
<html lang="pt">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Natureza Viva — Explorando o Mundo Natural</title>
  <meta name="description" content="Natureza Viva — artigos, fotografias e iniciativas de conservação. Descubra ecossistemas, espécies e como ajudar." />
  <style>
:root{
  --max-width:1100px;
  --accent:#2b8a67;
  --muted:#6b7280;
  --bg:#f7faf7;
  --text:#0f172a;
  --radius:12px;
  --glass: rgba(255,255,255,0.6);
  font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
}

*{box-sizing:border-box}
html,body{height:100%}
body{
  margin:0;
  color:var(--text);
  background:linear-gradient(180deg,#f1f6f4 0%,var(--bg) 100%);
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  line-height:1.45;
  font-size:16px;
}

.container{
  width:90%;
  max-width:var(--max-width);
  margin:0 auto;
  padding:3rem 0;
}

/* Header */
.site-header{
  background:rgba(255,255,255,0.7);
  backdrop-filter: blur(6px);
  position:sticky;
  top:0;
  z-index:50;
  box-shadow:0 1px 8px rgba(12,12,12,0.04);
}
.header-inner{
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:1rem;
  padding:0.75rem 0;
}
.logo{
  font-weight:700;
  color:var(--accent);
  text-decoration:none;
  font-size:1.1rem;
}
.main-nav{display:flex;gap:1rem;align-items:center}
.main-nav a{color:var(--muted);text-decoration:none;padding:0.4rem 0.6rem;border-radius:8px}
.main-nav a:hover{color:var(--text);background:var(--glass)}
.cta{background:var(--accent);color:white;padding:0.4rem 0.75rem}

/* Mobile toggle */
.nav-toggle{display:none;background:none;border:0;font-size:1.25rem}

/* Hero */
.hero{padding:3rem 0}
.hero-inner{display:grid;grid-template-columns:1fr 1fr;gap:2rem;align-items:center}
.hero-text h1{font-size:2.25rem;margin:0 0 .5rem}
.lead{color:var(--muted);margin-bottom:1rem}
.btn{display:inline-block;background:var(--accent);color:#fff;padding:.6rem 1rem;border-radius:10px;text-decoration:none}

/* Hero image */
.hero-image{
  height:320px;
  background-size:cover;
  background-position:center;
  border-radius:16px;
  box-shadow:0 10px 30px rgba(12,12,12,0.08);
}

/* Cards */
.cards{display:flex;gap:1rem;margin-top:1rem;flex-wrap:wrap}
.card{flex:1 1 220px;background:white;padding:1rem;border-radius:12px;box-shadow:0 6px 18px rgba(12,12,12,0.04)}

/* Grid */
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:1rem;margin-top:1rem}
.grid-item{background:white;padding:0.75rem;border-radius:12px;box-shadow:0 6px 18px rgba(12,12,12,0.04)}
.grid-item img{width:100%;height:150px;object-fit:cover;border-radius:8px}

/* species & list */
.species-list{list-style:none;padding:0;margin:0;display:grid;gap:.8rem}
.species-list li{background:white;padding:1rem;border-radius:10px;box-shadow:0 4px 12px rgba(12,12,12,0.04)}

/* gallery */
.masonry{display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
.masonry img{width:100%;height:140px;object-fit:cover;border-radius:8px}

/* two columns */
.two-col{display:grid;grid-template-columns:1fr 1fr;gap:1rem}

/* contact form */
.contact-form{display:grid;gap:.75rem;max-width:700px}
.contact-form label{display:block;font-size:.9rem;color:var(--muted)}
.contact-form input, .contact-form textarea{
  width:100%;padding:.6rem;border-radius:8px;border:1px solid #e6eef0;outline:none;font-size:1rem;
}
.form-message{color:var(--accent);margin-top:.5rem}

/* footer */
.site-footer{padding:1.5rem 0;background:#0b1320;color:#dbeafe}
.footer-inner{display:flex;justify-content:space-between;align-items:center;gap:1rem}
.site-footer a{color:#cfeee1;text-decoration:none}

/* Responsive */
@media (max-width:900px){
  .hero-inner{grid-template-columns:1fr}
  .grid{grid-template-columns:1fr 1fr}
  .masonry{grid-template-columns:repeat(2,1fr)}
  .main-nav{display:none}
  .nav-toggle{display:block}
}
@media (max-width:560px){
  .grid{grid-template-columns:1fr}
  .masonry{grid-template-columns:1fr}
  .two-col{grid-template-columns:1fr}
  .cards{flex-direction:column}
}
</style>
  <link rel="icon" href="assets/icons/favicon.png" />
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <a class="logo" href="#">Natureza Viva</a>
      <nav class="main-nav" aria-label="Navegação principal">
        <a href="#sobre">Sobre</a>
        <a href="#ecosistemas">Ecossistemas</a>
        <a href="#especies">Espécies</a>
        <a href="#galeria">Galeria</a>
        <a href="#conservacao">Conservação</a>
        <a href="#contacto" class="cta">Contacto</a>
      </nav>
      <button class="nav-toggle" aria-expanded="false" aria-controls="main-menu">☰</button>
    </div>
  </header>

  <main>
    <section class="hero" id="home" aria-label="Introdução">
      <div class="container hero-inner">
        <div class="hero-text">
          <h1>Natureza Viva</h1>
          <p>Descubra os ecossistemas do planeta, as espécies que o habitam e formas práticas de conservar a vida selvagem.</p>
          <a href="#ecosistemas" class="btn">Explorar ecossistemas</a>
        </div>
        <div class="hero-image" role="img" aria-label="Paisagem natural - montanhas e floresta" style="background-image:url('assets/images/hero.jpg')"></div>
      </div>
    </section>

    <section class="cards-section container" id="sobre">
      <h2>Sobre</h2>
      <p class="lead">A Natureza Viva é um espaço dedicado a informação de qualidade sobre ambiente, biodiversidade e conservação — para entusiastas, estudantes e profissionais.</p>
      <div class="cards">
        <article class="card">
          <h3>Missão</h3>
          <p>Informar e inspirar ações práticas para proteger habitats e espécies.</p>
        </article>
        <article class="card">
          <h3>Conteúdos</h3>
          <p>Artigos, guias, fotografias e notícias sobre biodiversidade.</p>
        </article>
        <article class="card">
          <h3>Comunidade</h3>
          <p>Projetos locais, voluntariado e parcerias com ONGs.</p>
        </article>
      </div>
    </section>

    <section class="ecosystems container" id="ecosistemas">
      <h2>Ecossistemas</h2>
      <p class="lead">Uma visão geral dos principais ecossistemas do planeta e suas características.</p>
      <div class="grid">
        <div class="grid-item">
          <img src="assets/images/forest.jpg" alt="Floresta densa" />
          <h4>Florestas</h4>
          <p>Altíssima biodiversidade; fundamentais para o ciclo da água e clima.</p>
        </div>
        <div class="grid-item">
          <img src="assets/images/ocean.jpg" alt="Mar aberto" />
          <h4>Oceano</h4>
          <p>Maior habitat do planeta; fonte de alimento e regulação climática.</p>
        </div>
        <div class="grid-item">
          <img src="assets/images/grassland.jpg" alt="Planície de savana" />
          <h4>Campos e Savanas</h4>
          <p>Habitat de grandes herbívoros e importantes para agricultura sustentável.</p>
        </div>
        <div class="grid-item">
          <img src="assets/images/wetland.jpg" alt="Área húmida" />
          <h4>Zonas Húmidas</h4>
          <p>Filtro natural da água e berçário para muitas espécies aquáticas.</p>
        </div>
      </div>
    </section>

    <section class="species container" id="especies">
      <h2>Espécies em Destaque</h2>
      <p class="lead">Algumas espécies emblemáticas e porque são importantes.</p>
      <ul class="species-list">
        <li>
          <h4>Tigre</h4>
          <p>Predador tope; sua presença indica ecossistemas saudáveis.</p>
        </li>
        <li>
          <h4>Abelha</h4>
          <p>Polinizadora essencial para segurança alimentar e biodiversidade.</p>
        </li>
        <li>
          <h4>Coral</h4>
          <p>Construções biológicas que sustentam vastas cadeias alimentares marinhas.</p>
        </li>
      </ul>
    </section>

    <section class="gallery container" id="galeria" aria-label="Galeria de fotografias">
      <h2>Galeria</h2>
      <div class="masonry">
        <img src="assets/images/gallery1.jpg" alt="Pássaro em voo" />
        <img src="assets/images/gallery2.jpg" alt="Riacho em floresta" />
        <img src="assets/images/gallery3.jpg" alt="Prado ao pôr do sol" />
        <img src="assets/images/gallery4.jpg" alt="Tartaruga marinha" />
      </div>
    </section>

    <section class="conservation container" id="conservacao">
      <h2>Conservação</h2>
      <p class="lead">Como pode ajudar — passos práticos e iniciativas recomendadas.</p>
      <div class="two-col">
        <div>
          <h3>Ações individuais</h3>
          <ul>
            <li>Reduzir consumo de plásticos descartáveis</li>
            <li>Plantar espécies nativas</li>
            <li>Consumir de forma sustentável</li>
          </ul>
        </div>
        <div>
          <h3>Envolver-se</h3>
          <ul>
            <li>Voluntariado em projetos locais</li>
            <li>Apoiar ONGs de conservação</li>
            <li>Educar a comunidade</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="contact container" id="contacto" aria-label="Formulário de contacto">
      <h2>Contacto</h2>
      <p class="lead">Tem perguntas, contribuições fotográficas ou quer colaborar? Envie uma mensagem.</p>
      <form id="contactForm" class="contact-form" method="post" action="#" novalidate>
        <label>
          Nome
          <input type="text" name="name" id="name" required />
        </label>
        <label>
          Email
          <input type="email" name="email" id="email" required />
        </label>
        <label>
          Mensagem
          <textarea name="message" id="message" rows="5" required></textarea>
        </label>
        <button type="submit" class="btn">Enviar mensagem</button>
        <p id="formMessage" class="form-message" aria-live="polite"></p>
      </form>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <p>© <span id="year"></span> Natureza Viva — Todos os direitos reservados.</p>
      <div class="social">
        <a href="#" aria-label="Instagram">IG</a>
        <a href="#" aria-label="Facebook">FB</a>
        <a href="#" aria-label="Twitter">TW</a>
      </div>
    </div>
  </footer>

  <script>
// Basic interactive behavior: nav toggle, contact form simple handling, year
document.addEventListener('DOMContentLoaded', function(){
  // Year in footer
  const y = document.getElementById('year');
  if(y) y.textContent = new Date().getFullYear();

  // Mobile nav toggle
  const toggle = document.querySelector('.nav-toggle');
  const nav = document.querySelector('.main-nav');
  if(toggle && nav){
    toggle.addEventListener('click', () => {
      const expanded = toggle.getAttribute('aria-expanded') === 'true';
      toggle.setAttribute('aria-expanded', String(!expanded));
      nav.style.display = expanded ? '' : 'flex';
    });
  }

  // Contact form basic validation & UX (client-side)
  const form = document.getElementById('contactForm');
  const formMessage = document.getElementById('formMessage');
  if(form){
    form.addEventListener('submit', function(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();

      if(!name || !email || !message){
        formMessage.textContent = 'Por favor preencha todos os campos.';
        formMessage.style.color = '#b91c1c';
        return;
      }
      // Simulação de envio: aqui podes ligar a um endpoint real (API)
      formMessage.style.color = '';
      formMessage.textContent = 'A mensagem foi enviada com sucesso. Obrigado!';
      form.reset();
      setTimeout(()=> formMessage.textContent = '', 5000);
    });
  }

  // Lazy-load images (simple)
  const imgs = document.querySelectorAll('img[data-src]');
  if('IntersectionObserver' in window){
    const obs = new IntersectionObserver((entries, observer)=>{
      entries.forEach(entry => {
        if(entry.isIntersecting){
          const img = entry.target;
          img.src = img.dataset.src;
          img.removeAttribute('data-src');
          observer.unobserve(img);
        }
      });
    });
    imgs.forEach(i => obs.observe(i));
  }
});
</script>
</body>
</html>