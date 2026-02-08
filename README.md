<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>José Carlos | Professional Footballer</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700;800&display=swap" rel="stylesheet">

<style>
:root{
  --black:#0b0b0b;
  --dark:#151515;
  --gold:#d4af37;
  --gold-light:#f1d77a;
}

*{box-sizing:border-box; scroll-behavior:smooth;}

body{
  margin:0;
  font-family:'Montserrat',sans-serif;
  background:var(--black);
  color:#fff;
}

/* ===== NAVBAR ===== */
nav{
  position:fixed;
  top:0;
  width:100%;
  padding:18px 60px;
  background:rgba(0,0,0,.55);
  backdrop-filter:blur(12px);
  display:flex;
  justify-content:space-between;
  align-items:center;
  z-index:999;
}

nav .logo{
  color:var(--gold);
  font-weight:800;
  letter-spacing:2px;
}

nav a{
  margin-left:25px;
  color:#fff;
  text-decoration:none;
  font-weight:500;
}

nav a:hover{color:var(--gold);}

.lang-btn{
  margin-left:30px;
  padding:6px 14px;
  border:1px solid var(--gold);
  color:var(--gold);
  cursor:pointer;
  font-size:13px;
}

/* ===== HERO ===== */
header{
  height:100vh;
  background:url("fotos/capa.jpg") center/cover no-repeat;
}

.hero{
  height:100%;
  background:rgba(0,0,0,.72);
  padding:120px 60px;
  display:flex;
  flex-direction:column;
  justify-content:center;
}

h1{
  font-size:72px;
  color:var(--gold);
  margin:0;
}

h2{
  font-size:28px;
  font-weight:300;
}

.hero p{
  max-width:780px;
  font-size:18px;
}

/* ===== BOTÕES ===== */
.btns a{
  display:inline-block;
  margin-top:30px;
  margin-right:20px;
  padding:14px 36px;
  border:2px solid var(--gold);
  color:var(--gold);
  text-decoration:none;
  font-weight:700;
  transition:.3s;
}

.btns a:hover{
  background:var(--gold);
  color:#000;
}

/* ===== SEÇÕES ===== */
section{
  padding:110px 60px;
  opacity:0;
  transform:translateY(40px);
  transition:.9s;
}

section.show{
  opacity:1;
  transform:translateY(0);
}

.title{
  font-size:34px;
  color:var(--gold);
  margin-bottom:40px;
}

/* ===== STATS ===== */
.stats{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
  gap:30px;
}

.stat{
  background:rgba(255,255,255,.05);
  border:1px solid rgba(212,175,55,.4);
  padding:30px;
  text-align:center;
  backdrop-filter:blur(10px);
}

.stat h3{
  font-size:42px;
  color:var(--gold);
  margin:0;
}

/* ===== PERFIL ===== */
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
  gap:25px;
}

.card{
  background:var(--dark);
  border-left:4px solid var(--gold);
  padding:25px;
  transition:.3s;
}

.card:hover{
  transform:translateY(-8px);
  box-shadow:0 15px 30px rgba(212,175,55,.25);
}

/* ===== GALERIA ===== */
.gallery{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:25px;
}

.gallery img,
.gallery video{
  width:100%;
  border-radius:10px;
  border:2px solid var(--gold);
  transition:.3s;
}

.gallery img:hover,
.gallery video:hover{
  transform:scale(1.05);
}

/* ===== FOOTER ===== */
footer{
  background:#000;
  text-align:center;
  padding:35px;
  color:#aaa;
}

a{color:var(--gold);}
</style>
</head>

<body>

<nav>
  <div class="logo">JC7</div>
  <div>
    <a href="#sobre" data-pt="Sobre" data-en="About">Sobre</a>
    <a href="#perfil" data-pt="Perfil" data-en="Profile">Perfil</a>
    <a href="#midia" data-pt="Highlights" data-en="Highlights">Highlights</a>
    <a href="#contato" data-pt="Contato" data-en="Contact">Contato</a>
    <span class="lang-btn" onclick="toggleLang()">PT / EN</span>
  </div>
</nav>

<header>
  <div class="hero">
    <h1>JOSÉ CARLOS</h1>
    <h2 data-pt="Lateral Direito" data-en="Right Back">Lateral Direito</h2>
    <p data-pt="Atleta moderno, intenso e disciplinado, com forte presença defensiva e apoio ofensivo constante pelo lado direito."
       data-en="Modern, intense and disciplined footballer, with strong defensive presence and constant offensive support on the right flank.">
       Atleta moderno, intenso e disciplinado, com forte presença defensiva e apoio ofensivo constante pelo lado direito.
    </p>

    <div class="btns">
      <a href="#perfil" data-pt="Perfil" data-en="Profile">Perfil</a>
      <a href="#midia" data-pt="Highlights" data-en="Highlights">Highlights</a>
    </div>
  </div>
</header>

<section id="sobre">
  <h3 class="title" data-pt="Sobre o Atleta" data-en="About the Player">Sobre o Atleta</h3>
  <p data-pt="José Carlos Santos de Souza é atleta de futebol, atua como lateral direito e se destaca pela intensidade, velocidade e disciplina tática. Busca evolução diária e alto rendimento profissional."
     data-en="José Carlos Santos de Souza is a football player who plays as a right back, standing out for intensity, speed and tactical discipline, focused on daily improvement and high performance.">
     José Carlos Santos de Souza é atleta de futebol, atua como lateral direito e se destaca pela intensidade, velocidade e disciplina tática. Busca evolução diária e alto rendimento profissional.
  </p>
</section>

<section>
  <div class="stats">
    <div class="stat"><h3 data-num="15">0</h3><p data-pt="Idade" data-en="Age">Idade</p></div>
    <div class="stat"><h3 data-num="172">0</h3><p data-pt="Altura (cm)" data-en="Height (cm)">Altura (cm)</p></div>
    <div class="stat"><h3 data-num="64">0</h3><p data-pt="Peso (kg)" data-en="Weight (kg)">Peso (kg)</p></div>
    <div class="stat"><h3 data-num="90">0</h3><p data-pt="Intensidade" data-en="Intensity">Intensidade</p></div>
  </div>
</section>

<section id="perfil">
  <h3 class="title" data-pt="Perfil Técnico" data-en="Technical Profile">Perfil Técnico</h3>
  <div class="grid">
    <div class="card" data-pt="⚽ Lateral Direito" data-en="⚽ Right Back">⚽ Lateral Direito</div>
    <div class="card" data-pt="🦵 Pé direito" data-en="🦵 Right foot">🦵 Pé direito</div>
    <div class="card" data-pt="🏃 Velocidade e resistência" data-en="🏃 Speed and endurance">🏃 Velocidade e resistência</div>
    <div class="card" data-pt="🛡️ Forte defesa" data-en="🛡️ Strong defense">🛡️ Forte defesa</div>
    <div class="card" data-pt="⚡ Apoio ofensivo" data-en="⚡ Offensive support">⚡ Apoio ofensivo</div>
    <div class="card" data-pt="📐 Disciplina tática" data-en="📐 Tactical discipline">📐 Disciplina tática</div>
  </div>
</section>

<section id="midia">
  <h3 class="title">Fotos & Highlights</h3>
  <div class="gallery">
    <img src="fotos/foto1.jpg">
    <img src="fotos/foto2.jpg">
    <video controls>
      <source src="videos/highlights.mp4" type="video/mp4">
    </video>
  </div>
</section>

<section id="contato">
  <h3 class="title" data-pt="Contato Profissional" data-en="Professional Contact">Contato Profissional</h3>
  <p>Email: jsantosdesouza446@gmail.com</p>
  <p>Instagram: <a href="https://instagram.com/jc.santoss7">@jc.santoss7</a></p>
</section>

<footer>
  © José Carlos Santos de Souza — Football Player
</footer>

<script>
/* Animações */
const sections=document.querySelectorAll("section");
window.addEventListener("scroll",()=>{
 sections.forEach(sec=>{
  if(sec.getBoundingClientRect().top<window.innerHeight-100){
    sec.classList.add("show");
  }
 });
});

/* Contadores */
document.querySelectorAll("[data-num]").forEach(counter=>{
 let started=false;
 window.addEventListener("scroll",()=>{
  if(counter.getBoundingClientRect().top<window.innerHeight && !started){
    started=true;
    let i=0, target=+counter.dataset.num;
    const interval=setInterval(()=>{
      i++; counter.innerText=i;
      if(i>=target) clearInterval(interval);
    },20);
  }
 });
});

/* Tradução */
let lang="pt";
function toggleLang(){
 lang = lang==="pt" ? "en" : "pt";
 document.querySelectorAll("[data-pt]").forEach(el=>{
   el.innerText = el.dataset[lang];
 });
}
</script>

</body>
</html>
