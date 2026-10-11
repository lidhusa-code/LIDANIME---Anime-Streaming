<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>LIDANIME — Anime Universe</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#090912;color:#f5f5ff;font-family:Arial,sans-serif}
header{padding:20px 5%;display:flex;justify-content:space-between;align-items:center;background:#11111d;position:sticky;top:0;z-index:5}
.logo{font-size:25px;font-weight:900;color:#a78bfa}
.logo span{color:white}
nav a{color:#ddd;text-decoration:none;margin-left:14px;font-size:13px}
.hero{padding:65px 6%;background:linear-gradient(90deg,#100b27,#28104b,#101020);min-height:290px}
.tag{color:#c4b5fd;font-size:12px;letter-spacing:3px}
h1{font-size:42px;margin:14px 0}
.hero p{color:#d0cde0;max-width:460px;line-height:1.6}
.btn{display:inline-block;padding:12px 18px;background:#8b5cf6;color:white;border:0;border-radius:8px;text-decoration:none;font-weight:bold;cursor:pointer}
section{padding:25px 5%}
.tools{display:flex;gap:10px;flex-wrap:wrap;margin:16px 0}
input,select{padding:12px;border-radius:8px;border:1px solid #39334d;background:#171523;color:white}
input{flex:1;min-width:170px}
.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:13px}
.card{background:#151421;border:1px solid #272338;border-radius:12px;overflow:hidden}
.poster{height:145px;display:flex;align-items:center;justify-content:center;text-align:center;font-size:22px;font-weight:900;padding:10px;background:linear-gradient(140deg,#312e81,#7e22ce,#111827)}
.card h3{font-size:14px;margin:12px 10px 5px}
.card p{font-size:12px;color:#aaa;margin:5px 10px 12px}
.card button{margin:0 10px 13px}
.notice{color:#aaa;font-size:12px;line-height:1.6}
footer{text-align:center;padding:30px;color:#999;background:#11111d;font-size:12px}
@media(min-width:700px){.grid{grid-template-columns:repeat(4,minmax(0,1fr))}.poster{height:210px}}
</style>
</head>
<body>
<header>
  <div class="logo">LID<span>ANIME</span></div>
  <nav><a href="#home">Home</a><a href="#anime">Anime</a></nav>
</header>
<div class="hero" id="home">
  <div class="tag">WELCOME TO YOUR ANIME UNIVERSE</div>
  <h1>Enter The Anime World.</h1>
  <p>Temukan anime favoritmu, jelajahi berbagai genre, dan nikmati petualangan tanpa batas.</p>
  <a class="btn" href="#anime">Jelajahi Anime ↗</a>
</div>
<section id="anime">
  <h2>Jelajahi Anime</h2>
  <div class="tools">
    <input id="search" placeholder="Cari judul anime..." oninput="filterAnime()">
    <select id="genre" onchange="filterAnime()">
      <option value="all">Semua Genre</option>
      <option value="Action">Action</option>
      <option value="Fantasy">Fantasy</option>
      <option value="Adventure">Adventure</option>
    </select>
  </div>
  <div class="grid" id="grid"></div>
  <p class="notice">Katalog demo. Poster dan video dapat ditambahkan melalui sumber resmi yang memiliki izin.</p>
</section>
<footer>© 2026 LIDANIME · Anime Universe<br>Fan discovery website — bukan pemilik hak cipta anime.</footer>
<script>
const anime=[
 {name:"Martial Peak",genre:"Action",desc:"Cultivation • Martial Arts"},
 {name:"Battle Through the Heavens",genre:"Fantasy",desc:"Fantasy • Adventure"},
 {name:"Soul Land",genre:"Adventure",desc:"Action • Fantasy"},
 {name:"Perfect World",genre:"Action",desc:"Cultivation • Fantasy"},
 {name:"Swallowed Star",genre:"Fantasy",desc:"Sci-Fi • Action"},
 {name:"Throne of Seal",genre:"Adventure",desc:"Fantasy • Adventure"}
];
function filterAnime(){
 const q=document.getElementById("search").value.toLowerCase();
 const g=document.getElementById("genre").value;
 document.getElementById("grid").innerHTML=anime.filter(a=>
 a.name.toLowerCase().includes(q)&&(g==="all"||a.genre===g)
 ).map(a=>`<article class="card">
 <div class="poster">${a.name}</div>
 <h3>${a.name}</h3><p>${a.desc}</p>
 <button class="btn" onclick="alert('Tambahkan tautan video resmi untuk '+${JSON.stringify(a.name)})">Lihat Anime</button>
 </article>`).join("");
}
filterAnime();
</script>
</body>
</html>
