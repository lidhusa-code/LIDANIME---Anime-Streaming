
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#0b0913">
<title>LIDANIME — Anime Universe</title>
<style>
:root{--bg:#0b0913;--panel:#171321;--purple:#a78bfa;--text:#f7f4ff;--muted:#aaa2bb}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--text);font-family:Arial,sans-serif}
header{padding:20px 5%;background:#100d1b;border-bottom:1px solid #30263f;position:sticky;top:0;z-index:5}
.top{display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
.logo{font-size:25px;font-weight:900;letter-spacing:1px;color:var(--purple)}
.logo span{color:white}
.tagline{font-size:12px;color:var(--muted);margin-top:5px}
.search{width:100%;margin-top:17px;padding:13px 15px;border:1px solid #393047;border-radius:12px;background:#1c1727;color:white;font-size:15px;outline:none}
.search:focus{border-color:var(--purple)}
main{padding:22px 5%;max-width:1500px;margin:auto}
.hero{padding:27px 22px;border-radius:18px;background:linear-gradient(120deg,#30204b,#151020 70%);margin-bottom:25px}
.hero h1{font-size:clamp(25px,5vw,42px);margin:0 0 10px}
.hero p{color:#d0c5e1;line-height:1.6;margin:0}
.section-head{display:flex;align-items:center;justify-content:space-between;gap:10px;margin:25px 0 15px}
.section-head h2{font-size:20px;margin:0}
#status{color:var(--muted);font-size:13px}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(135px,1fr));gap:15px}
.card{cursor:pointer;min-width:0;background:var(--panel);border:1px solid #292235;border-radius:12px;overflow:hidden;transition:.2s}
.card:hover{transform:translateY(-4px);border-color:var(--purple)}
.card img{width:100%;aspect-ratio:3/4;object-fit:cover;display:block;background:#211a2d}
.card-info{padding:10px}
.card h3{font-size:14px;line-height:1.4;margin:0 0 7px}
.card p{font-size:12px;color:var(--muted);margin:0}
.btn{border:0;border-radius:9px;background:var(--purple);color:#160e25;padding:11px 15px;font-weight:bold;cursor:pointer;text-decoration:none;display:inline-block}
.btn.secondary{background:#2a2338;color:white;border:1px solid #49405b}
button:disabled{opacity:.5}
#detail{margin-top:25px;padding:18px;background:var(--panel);border:1px solid #352a47;border-radius:16px}
.detail-top{display:grid;grid-template-columns:minmax(110px,190px) 1fr;gap:20px}
#poster{width:100%;border-radius:12px;aspect-ratio:3/4;object-fit:cover;background:#211a2d}
#detail h2{margin:0 0 10px;font-size:24px}
.meta{font-size:13px;color:var(--muted);line-height:1.7}
.description{font-size:14px;line-height:1.7;color:#e0d9eb}
.actions{display:flex;flex-wrap:wrap;gap:9px;margin:15px 0}
.player{margin-top:22px;padding:14px;background:#0c0a12;border:1px solid #352a47;border-radius:14px}
.player h3{margin:0 0 14px}
video{display:block;width:100%;aspect-ratio:16/9;background:#000;border-radius:10px}
.player select{width:100%;padding:12px;margin-top:12px;border-radius:9px;background:#211a2d;border:1px solid #49405b;color:white}
#playerStatus{font-size:13px;color:var(--muted);line-height:1.5}
.hidden{display:none!important}
footer{text-align:center;padding:30px 15px;color:var(--muted);font-size:12px}
.empty{grid-column:1/-1;padding:24px;text-align:center;color:var(--muted);background:var(--panel);border-radius:12px}
@media(max-width:550px){main{padding:17px 4%}.grid{grid-template-columns:repeat(2,minmax(0,1fr));gap:12px}.detail-top{grid-template-columns:110px 1fr;gap:13px}#detail h2{font-size:19px}.hero{padding:22px 17px}}
</style>
</head>
<body>
<header>
  <div class="top">
    <div>
      <div class="logo">LID<span>ANIME</span></div>
      <div class="tagline">Your Anime Universe · Discover your next story</div>
    </div>
    <button class="btn secondary" onclick="loadAnime()">↻ Refresh</button>
  </div>
  <input id="search" class="search" placeholder="Cari anime favorit kamu..." autocomplete="off">
</header>

<main>
  <section class="hero">
    <h1>Enter Your Anime World.</h1>
    <p>Temukan anime favorit, jelajahi genre, lihat detail cerita, dan putar video yang tersedia.</p>
  </section>

  <div class="section-head">
    <h2>🔥 Anime Populer</h2>
    <span id="status">Memuat anime...</span>
  </div>
  <div id="catalog" class="grid"></div>

  <section id="detail" class="hidden">
    <div class="detail-top">
      <img id="poster" alt="Poster anime">
      <div>
        <h2 id="animeTitle">Detail Anime</h2>
        <div id="animeMeta" class="meta"></div>
        <p id="animeDescription" class="description"></p>
      </div>
    </div>

    <div class="actions">
      <a id="officialLink" class="btn" href="#" target="_blank" rel="noopener">Cari Streaming Resmi ↗</a>
      <a id="aniListLink" class="btn secondary" href="#" target="_blank" rel="noopener">Info Lengkap ↗</a>
    </div>

    <div class="player">
      <h3>🎬 LIDANIME Player</h3>
      <video id="animeVideo" controls playsinline preload="metadata">
        Browser kamu tidak mendukung pemutar video.
      </video>
      <select id="episodeSelect" aria-label="Pilih episode">
        <option value="">Pilih episode</option>
      </select>
      <p id="playerStatus">Pilih anime untuk melihat video yang tersedia.</p>
    </div>
    <div class="actions">
      <button class="btn secondary" onclick="closeDetail()">✕ Tutup Detail</button>
    </div>
  </section>
</main>

<footer>
  LIDANIME © 2026 · Informasi anime dari AniList API.<br>
  Video harus berasal dari sumber yang kamu miliki atau berhak gunakan.
</footer>

<script>
const API = "https://graphql.anilist.co";

/*
  TAMBAHKAN VIDEO DI SINI.
  Ganti ID anime dengan ID AniList yang sesuai.
  URL harus berupa URL file video langsung yang sah,
  misalnya file MP4 yang kamu miliki atau berhak putar.

  Contoh format:
  "ID_ANIME": [
    { title: "Episode 1", url: "https://domainmu.com/video1.mp4" },
    { title: "Episode 2", url: "https://domainmu.com/video2.mp4" }
  ]
*/
const VIDEO_LIBRARY = {
  // "ID_ANIME": [
  //   { title: "Episode 1", url: "URL_VIDEO_MP4_KAMU" }
  // ]
};

const catalog = document.getElementById("catalog");
const statusText = document.getElementById("status");
const searchInput = document.getElementById("search");
const detail = document.getElementById("detail");
const video = document.getElementById("animeVideo");
const episodeSelect = document.getElementById("episodeSelect");
const playerStatus = document.getElementById("playerStatus");

let searchTimer;
let requestNumber = 0;

const QUERY = `
query ($search: String, $page: Int) {
  Page(page: $page, perPage: 24) {
    media(search: $search, type: ANIME, sort: POPULARITY_DESC) {
      id
      title { romaji english native }
      coverImage { large extraLarge }
      episodes
      averageScore
      seasonYear
      format
      genres
      description(asHtml: false)
      siteUrl
    }
  }
}`;

async function fetchAnime(search = "") {
  const res = await fetch(API, {
    method: "POST",
    headers: { "Content-Type": "application/json", "Accept": "application/json" },
    body: JSON.stringify({
      query: QUERY,
      variables: { search: search || null, page: 1 }
    })
  });
  if (!res.ok) throw new Error("API tidak merespons");
  const json = await res.json();
  if (json.errors) throw new Error("Data anime gagal dimuat");
  return json.data.Page.media;
}

function escapeHTML(value = "") {
  return String(value).replace(/[&<>"']/g, c => ({
    "&":"&amp;", "<":"&lt;", ">":"&gt;", '"':"&quot;", "'":"&#39;"
  }[c]));
}

function titleOf(a) {
  return a.title.english || a.title.romaji || a.title.native || "Anime";
}

function renderCatalog(list) {
  catalog.innerHTML = "";
  if (!list.length) {
    catalog.innerHTML = '<div class="empty">Anime tidak ditemukan. Coba kata kunci lain.</div>';
    return;
  }

  list.forEach(a => {
    const card = document.createElement("article");
    card.className = "card";
    card.tabIndex = 0;
    card.innerHTML = `
      <img loading="lazy" src="${escapeHTML(a.coverImage.extraLarge || a.coverImage.large || "")}" alt="Poster ${escapeHTML(titleOf(a))}">
      <div class="card-info">
        <h3>${escapeHTML(titleOf(a))}</h3>
        <p>${a.seasonYear || "Tahun tidak diketahui"} · ★ ${a.averageScore ? (a.averageScore / 10).toFixed(1) : "N/A"}</p>
      </div>`;
    card.onclick = () => showDetail(a);
    card.onkeydown = e => {
      if (e.key === "Enter") showDetail(a);
    };
    catalog.appendChild(card);
  });
}

async function loadAnime(search = "") {
  const currentRequest = ++requestNumber;
  statusText.textContent = "Memuat...";
  catalog.innerHTML = '<div class="empty">Sedang mengambil katalog anime...</div>';

  try {
    const list = await fetchAnime(search);
    if (currentRequest !== requestNumber) return;
    renderCatalog(list);
    statusText.textContent = list.length + " anime ditemukan";
  } catch (err) {
    if (currentRequest !== requestNumber) return;
    catalog.innerHTML = '<div class="empty">Gagal memuat katalog. Periksa koneksi internet lalu tekan Refresh.</div>';
    statusText.textContent = "Koneksi bermasalah";
  }
}

function showDetail(a) {
  detail.classList.remove("hidden");
  document.getElementById("poster").src = a.coverImage.extraLarge || a.coverImage.large || "";
  document.getElementById("animeTitle").textContent = titleOf(a);
  document.getElementById("animeMeta").textContent =
    `${a.format || "Anime"} · ${a.seasonYear || "Tahun tidak diketahui"} · ${a.episodes || "?"} episode · Skor ${a.averageScore ? (a.averageScore / 10).toFixed(1) : "N/A"} · ${(a.genres || []).join(", ")}`;
  document.getElementById("animeDescription").textContent =
    (a.description || "Belum ada deskripsi.").replace(/<[^>]*>/g, "");
  document.getElementById("officialLink").href =
    "https://www.justwatch.com/id/search?q=" + encodeURIComponent(titleOf(a));
  document.getElementById("aniListLink").href = a.siteUrl || "https://anilist.co";

  loadVideos(a.id);
  detail.scrollIntoView({ behavior: "smooth", block: "start" });
}

function loadVideos(animeId) {
  video.pause();
  video.removeAttribute("src");
  video.load();
  episodeSelect.innerHTML = "";

  const episodes = VIDEO_LIBRARY[String(animeId)] || [];

  if (!episodes.length) {
    episodeSelect.add(new Option("Video belum ditambahkan", ""));
    playerStatus.textContent =
      "Belum ada URL video untuk anime ini. Tambahkan video yang sah di VIDEO_LIBRARY pada kode.";
    return;
  }

  episodes.forEach((ep, index) => {
    episodeSelect.add(new Option(ep.title || `Episode ${index + 1}`, String(index)));
  });

  episodeSelect.onchange = () => {
    const ep = episodes[Number(episodeSelect.value)];
    if (!ep) return;
    video.pause();
    video.src = ep.url;
    video.load();
    playerStatus.textContent = "Memuat " + (ep.title || "episode") + "...";
  };

  video.oncanplay = () => {
    playerStatus.textContent = "Video siap diputar.";
  };
  video.onerror = () => {
    playerStatus.textContent =
      "Video gagal diputar. Pastikan URL benar, file tersedia, dan server mengizinkan pemutaran.";
  };

  episodeSelect.value = "0";
  episodeSelect.onchange();
}

function closeDetail() {
  video.pause();
  detail.classList.add("hidden");
}

searchInput.addEventListener("input", () => {
  clearTimeout(searchTimer);
  searchTimer = setTimeout(() => loadAnime(searchInput.value.trim()), 450);
});

loadAnime();
</script>
</body>
</html>
