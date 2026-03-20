<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pastelaria Doce Sabor</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #C9A84C;
  --gold-light: #F0D080;
  --gold-dim: #6b5720;
  --black: #050403;
}

* { margin:0; padding:0; box-sizing:border-box; }

body {
  font-family: 'DM Sans', sans-serif;
  color: #fff;
  background: var(--black);
  overflow-x: hidden;
}

h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(32px, 8vw, 72px);
  font-weight: 400;
  color: var(--gold-light);
  line-height: 1.1;
  margin-bottom: 16px;
  text-shadow: 0 2px 24px rgba(0,0,0,0.8);
}
h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(26px, 6vw, 54px);
  font-weight: 400;
  color: var(--gold-light);
  line-height: 1.15;
  margin-bottom: 14px;
}
p {
  font-size: clamp(13px, 3vw, 16px);
  color: rgba(255,255,255,0.7);
  line-height: 1.8;
  margin: 12px 0;
  font-weight: 300;
}

.label {
  font-size: 10px;
  letter-spacing: 5px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 12px;
  display: block;
}

button {
  padding: 13px 36px;
  font-family: 'DM Sans', sans-serif;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 2.5px;
  text-transform: uppercase;
  background: var(--gold);
  color: #000;
  border: none;
  cursor: pointer;
  margin: 8px;
  transition: all 0.3s;
  clip-path: polygon(8px 0%, 100% 0%, calc(100% - 8px) 100%, 0% 100%);
}
button:hover {
  background: var(--gold-light);
  transform: translateY(-2px);
  box-shadow: 0 12px 32px rgba(201,168,76,0.3);
}
button.btn-outline {
  background: transparent;
  color: var(--gold);
  border: 1px solid var(--gold-dim);
}
button.btn-outline:hover {
  background: rgba(201,168,76,0.08);
  border-color: var(--gold);
}

.page {
  width: 100%;
  min-height: 100vh;
  display: none;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-size: cover;
  background-position: center;
  animation: fadeIn 0.8s ease;
  padding: 20px;
  position: relative;
}
.page::before {
  content: '';
  position: absolute; inset: 0;
  background: rgba(5,4,3,0.78);
}
.active { display: flex; }

.overlay {
  background: rgba(0,0,0,0.55);
  border: 1px solid rgba(201,168,76,0.15);
  padding: clamp(28px, 6vw, 60px);
  width: 100%;
  max-width: 780px;
  position: relative;
  z-index: 1;
}
.overlay::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
}

.gold-line {
  width: 48px; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 18px auto;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(12px); }
  to   { opacity: 1; transform: translateY(0); }
}

.btn-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 4px;
  margin-top: 20px;
}

/* MENU */
.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 12px;
  margin: 20px 0;
}
.menu-item {
  border: 1px solid rgba(201,168,76,0.2);
  padding: 14px 10px;
  background: rgba(201,168,76,0.04);
  transition: all 0.3s;
}
.menu-item:hover {
  border-color: rgba(201,168,76,0.5);
  background: rgba(201,168,76,0.08);
}
.menu-item .icon { font-size: 24px; margin-bottom: 6px; }
.menu-item .name {
  font-family: 'Playfair Display', serif;
  font-size: clamp(12px, 3vw, 15px);
  color: var(--gold-light);
  font-style: italic;
}
</style>
</head>
<body>

<!-- PÁGINA 1 — ENTRADA -->
<div id="p1" class="page active"
style="background-image:url('https://images.pexels.com/photos/205961/pexels-photo-205961.jpeg');">
  <div class="overlay">
    <span class="label">°•°.Artesanal & Elegante</span>
    <h1>🍰 Pastelaria<br>Doce Sabor</h1>
    <div class="gold-line"></div>
    <p>Uma tradição de sabor, requinte e excelência artesanal.<br>
    Doces, bolos e salgados feitos com amor.</p>
    <div class="btn-group">
      <button onclick="goTo('p2')">Entrar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 2 — SOBRE -->
<div id="p2" class="page"
style="background-image:url('https://images.pexels.com/photos/1307698/pexels-photo-1307698.jpeg');">
  <div class="overlay">
    <span class="label">A nossa história</span>
    <h2>🏠 Sobre Nós</h2>
    <div class="gold-line"></div>
    <p>Fundada com paixão e dedicação, a Doce Sabor é um espaço onde
    a confeitaria artesanal encontra a elegância do detalhe.</p>
    <p>Cada criação é elaborada com ingredientes cuidadosamente selecionados,
    honrando o sabor autêntico e a excelência em cada peça.</p>
    <div class="btn-group">
      <button onclick="goTo('p3')">Ver Menu</button>
      <button class="btn-outline" onclick="goTo('p1')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 3 — MENU -->
<div id="p3" class="page"
style="background-image:url('https://images.pexels.com/photos/239578/pexels-photo-239578.jpeg');">
  <div class="overlay">
    <span class="label">O que oferecemos</span>
    <h2>🍩 Nosso Menu</h2>
    <div class="gold-line"></div>
    <div class="menu-grid">
      <div class="menu-item"><div class="icon">🍰</div><div class="name">Bolo de Chocolate</div></div>
      <div class="menu-item"><div class="icon">🎂</div><div class="name">Bolo Red Velvet</div></div>
      <div class="menu-item"><div class="icon">🍩</div><div class="name">Donuts</div></div>
      <div class="menu-item"><div class="icon">🥐</div><div class="name">Croissant</div></div>
      <div class="menu-item"><div class="icon">🥟</div><div class="name">Salgados</div></div>
      <div class="menu-item"><div class="icon">🥪</div><div class="name">Sanduíches</div></div>
      <div class="menu-item"><div class="icon">🍮</div><div class="name">Pudim</div></div>
      <div class="menu-item"><div class="icon">🍪</div><div class="name">Cookies</div></div>
    </div>
    <div class="btn-group">
      <button onclick="goTo('p4')">Galeria</button>
      <button class="btn-outline" onclick="goTo('p2')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 4 — GALERIA -->
<div id="p4" class="page"
style="background-image:url('https://images.pexels.com/photos/1126359/pexels-photo-1126359.jpeg');">
  <div class="overlay">
    <span class="label">Galeria</span>
    <h2>🎥 As Nossas Criações</h2>
    <div class="gold-line"></div>
    <p>Uma seleção das nossas criações — onde o sabor se torna arte.</p>

    <iframe src="https://drive.google.com/file/d/1hDEoBrPzhVs1MTgM36YKRFuqy7Oq1YRP/preview"
      width="100%" height="220" allow="autoplay"
      style="border:1px solid rgba(201,168,76,0.2);margin:10px 0;border-radius:4px;"></iframe>

    <iframe src="https://drive.google.com/file/d/10Z3VDxRl1htSYNmZy_kj08cNongdGyWh/preview"
      width="100%" height="220" allow="autoplay"
      style="border:1px solid rgba(201,168,76,0.2);margin:10px 0;border-radius:4px;"></iframe>

    <iframe src="https://drive.google.com/file/d/1NSfFr-uC-Jcv-IY8C-LBolGwc-fW2TyQ/preview"
      width="100%" height="220" allow="autoplay"
      style="border:1px solid rgba(201,168,76,0.2);margin:10px 0;border-radius:4px;"></iframe>

    <iframe src="https://drive.google.com/file/d/1DNWwdb7k4JCBD2LulQDJF3m1Id3IeMoC/preview"
      width="100%" height="220" allow="autoplay"
      style="border:1px solid rgba(201,168,76,0.2);margin:10px 0;border-radius:4px;"></iframe>

    <div class="btn-group">
      <button onclick="goTo('p5')">Contacto</button>
      <button class="btn-outline" onclick="goTo('p3')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 5 — CONTACTO -->
<div id="p5" class="page"
style="background-image:url('https://images.pexels.com/photos/1395967/pexels-photo-1395967.jpeg');">
  <div class="overlay">
    <span class="label">Encomendas & Marcações</span>
    <h2>📍 Contacto</h2>
    <div class="gold-line"></div>
    <p>Estamos sempre prontos para o servir.<br>
    Faça a sua encomenda diretamente pelo WhatsApp.</p>

    <iframe
      src="https://www.google.com/maps?q=Lisboa&output=embed"
      width="100%" height="220"
      style="border:1px solid rgba(201,168,76,0.2);margin:16px 0;">
    </iframe>

    <div class="btn-group">
      <a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Quero%20encomendar%20doces%20e%20salgados.🍰🥪" target="_blank">
        <button>WhatsApp</button>
      </a>
      <button class="btn-outline" onclick="goTo('p4')">Voltar</button>
    </div>
  </div>
</div>

<script>
function goTo(page) {
  document.querySelector('.active').classList.remove('active');
  document.getElementById(page).classList.add('active');
  window.scrollTo(0,0);
}
</script>
</body>
</html>

