<html lang="pt">
<head>
<meta charset="UTF-8">
<title>Pastelaria Doce Sabor</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Garamond:wght@300;400;500&display=swap" rel="stylesheet">

<style>

*{margin:0;padding:0;box-sizing:border-box;}

body{
font-family:'Cormorant Garamond', serif;
background:black;
color:gold;
overflow-x:hidden;
}

/* TEXTOS */
h1{
font-family:'Playfair Display', serif;
font-size:90px;
text-shadow:3px 3px 30px rgba(0,0,0,0.9);
letter-spacing:2px;
line-height:1.1;
}
h2{font-size:70px;margin-bottom:20px;}
p{
font-size:32px;
margin:20px 0;
font-weight:300;
letter-spacing:1px;
line-height:1.5;
}

/* BOTÕES */
button{
padding:22px 50px;
font-size:22px;
font-family:'Cormorant Garamond', serif;
font-weight:500;
letter-spacing:2px;
text-transform:uppercase;
background:transparent;
color:gold;
border:1px solid gold;
border-radius:0;
cursor:pointer;
margin:10px;
transition:0.4s;
}

button:hover{
background:gold;
color:#1a0e00;
transform:scale(1.05);
box-shadow:0 0 30px rgba(255,215,0,0.4);
}

/* PÁGINAS */
.page{
width:100%;
height:100vh;
display:none;
justify-content:center;
align-items:center;
text-align:center;
background-size:cover;
background-position:center;
position:relative;
}

.page::before{
content:'';
position:absolute;
inset:0;
background:rgba(10,6,0,0.60);
}

.active{
display:flex;
}

/* CAIXA CENTRAL */
.overlay{
position:relative;
z-index:2;
background:rgba(10,6,0,0.72);
padding:60px 70px;
border:1px solid rgba(255,215,0,0.25);
width:90%;
max-width:1100px;
box-shadow:0 0 60px rgba(0,0,0,0.8), inset 0 0 40px rgba(255,215,0,0.03);
}

/* Linha decorativa dourada acima e abaixo do título */
.overlay h1::before,
.overlay h1::after{
content:'— ✦ —';
display:block;
font-size:22px;
letter-spacing:8px;
color:rgba(255,215,0,0.55);
margin:12px 0;
font-family:'Cormorant Garamond', serif;
font-style:italic;
}

/* VÍDEOS */
video{
width:100%;
max-width:820px;
border-radius:0;
margin:14px 0;
border:1px solid rgba(255,215,0,0.2);
}

/* MENU DOCES */
.menu{
font-size:30px;
line-height:58px;
font-family:'Cormorant Garamond', serif;
font-weight:400;
letter-spacing:1px;
}

/* SEPARADOR */
.sep{
width:120px;
height:1px;
background:rgba(255,215,0,0.4);
margin:25px auto;
}

</style>
</head>

<body>

<!-- PÁGINA 1 -->
<div id="p1" class="page active"
style="background-image:url('https://images.pexels.com/photos/205961/pexels-photo-205961.jpeg');">
<div class="overlay">
  <h1>🍰Pastelaria<br>Doce Sabor</h1>
  <div class="sep"></div>
  <p>Uma tradição de sabor, requinte e excelência artesanal.<p>
    Doces, bolos e salgados feitos com amor.</p>
  <br>
  <button onclick="go('p2')">Entrar</button>
</div>
</div>


<!-- PÁGINA 2 SOBRE -->
<div id="p2" class="page"
style="background-image:url('https://images.pexels.com/photos/1307698/pexels-photo-1307698.jpeg');">
<div class="overlay">
  <h1>🏠Sobre Nós</h1>
  <div class="sep"></div>
  <p>Fundada com paixão e dedicação, a Doce Sabor é um espaço onde<br>
  a confeitaria artesanal encontra a elegância do detalhe.<br>
  <p>Cada criação é elaborada com ingredientes cuidadosamente selecionados,<br>
  honrando o sabor autêntico e a excelência em cada peça.<p>
    Trabalhamos com ingredientes de qualidade
para oferecer a melhor experiência aos nossos clientes.</p>
  <br>
  <button onclick="go('p3')">Menu</button>
  <button onclick="go('p1')">Voltar</button>
</div>
</div>


<!-- PÁGINA 3 MENU -->
<div id="p3" class="page"
style="background-image:url('https://images.pexels.com/photos/239578/pexels-photo-239578.jpeg');">
<div class="overlay">
  <h1>🍩Nosso Menu</h1>
  <div class="sep"></div>
  <div class="menu">
    🍰 Bolo de Chocolate &nbsp;·&nbsp; 🍰 Bolo Red Velvet<br>
    🍩 Donuts &nbsp;·&nbsp; 🥐 Croissant<br>
    🥟 Salgados &nbsp;·&nbsp; 🥪 Sanduíches<br>
    🍮 Pudim &nbsp;·&nbsp; 🍪 Cookies
  </div>
  <br>
  <button onclick="go('p4')">Galeria</button>
  <button onclick="go('p2')">Voltar</button>
</div>
</div>


<!-- PÁGINA 4 GALERIA -->
<div id="p4" class="page"
style="background-image:url('https://images.pexels.com/photos/1126359/pexels-photo-1126359.jpeg');">
<div class="overlay">
  <h1>🎥Galeria</h1>
  <div class="sep"></div>
  <p>Uma seleção das nossas criações — onde o sabor se torna arte. <br>
  <p>Veja os nossos doces e salgados.</p>

  <iframe 
  src="https://drive.google.com/file/d/1hDEoBrPzhVs1MTgM36YKRFuqy7Oq1YRP/preview?usp=sharing" 
  width="100%" 
  height="315"
  allow="autoplay"
  allowfullscreen
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>

  <iframe 
  src="https://drive.google.com/file/d/10Z3VDxRl1htSYNmZy_kj08cNongdGyWh/preview?uso=sharing"
  width="100%" 
  height="315"
  allow="autoplay"
  allowfullscreen
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>
  
  <iframe 
  src="https://drive.google.com/file/d/1NSfFr-uC-Jcv-IY8C-LBolGwc-fW2TyQ/preview?uso=sharing" 
  width="100%" 
  height="315"allow="autoplay"
  allowfullscreen
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>
  
  <iframe 
  src="https://drive.google.com/file/d/1DNWwdb7k4JCBD2LulQDJF3m1Id3IeMoC/preview?uso=sharing"
  width="100%" 
  height="315"allow="autoplay"
  allowfullscreen
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>

  <br>
  <button onclick="go('p5')">Contacto</button>
  <button onclick="go('p3')">Voltar</button>
</div>
</div>


<!-- PÁGINA 5 CONTATO -->
<div id="p5" class="page"
style="background-image:url('https://images.pexels.com/photos/1395967/pexels-photo-1395967.jpeg');">
<div class="overlay">
  <h1>📍Contacto</h1>
  <div class="sep"></div>
  <p>Receba-nos de portas abertas — estamos sempre prontos para o servir. <br>
  <p>Venha visitar a nossa pastelaria.</p>

  <iframe
    src="https://www.google.com/maps?q=Lisboa&output=embed"
    width="100%"
    height="280"
    style="border:0;border:1px solid rgba(255,215,0,0.2);margin:10px 0;">
  </iframe>

  <br><br>

  <a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Quero%20encomendar%20doces%20e%20salgados.🍰🥪" target="_blank">
    <button>WhatsApp</button>
  </a>
  <button onclick="go('p4')">Voltar</button>
</div>
</div>


<script>
function go(page){
  document.querySelector('.active').classList.remove('active');
  document.getElementById(page).classList.add('active');
}
</script>

</body>
</html>
