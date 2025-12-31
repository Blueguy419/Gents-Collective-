<!doctype html>  
<html lang="en">  
<head>  
  <meta charset="utf-8" />  
  <meta name="viewport" content="width=device-width,initial-scale=1" />  
  <meta name="description" content="Gents Collective — clean, modern streetwear. Oversized tees, baggy jeans, and heavy oversized hoodies." />  
  <meta name="theme-color" content="#0b0b0b" />  
  <title>Gents Collective</title>  
  
  <style>  
    :root{  
      --bg:#0b0b0b;  
      --panel:#111;  
      --text:#f5f5f5;  
      --muted:#b9b9b9;  
      --line:rgba(255,255,255,.12);  
      --accent:#2cff8f; /* modern green accent */  
      --shadow: 0 12px 30px rgba(0,0,0,.45);  
      --radius: 18px;  
      --radius2: 28px;  
      --max: 1100px;  
      --font: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";  
    }  
  
    *{box-sizing:border-box}  
    html,body{height:100%}  
    body{  
      margin:0;  
      font-family: var(--font);  
      background:  
        radial-gradient(1200px 800px at 15% 10%, rgba(44,255,143,.12), transparent 50%),  
        radial-gradient(900px 700px at 90% 15%, rgba(255,255,255,.06), transparent 55%),  
        var(--bg);  
      color:var(--text);  
      line-height:1.45;  
      letter-spacing:.2px;  
    }  
  
    a{color:inherit; text-decoration:none}  
    .wrap{max-width:var(--max); margin:0 auto; padding:24px}  
    .pill{  
      display:inline-flex; align-items:center; gap:10px;  
      padding:10px 14px;  
      border:1px solid var(--line);  
      border-radius:999px;  
      background: rgba(255,255,255,.03);  
      backdrop-filter: blur(8px);  
    }  
    .dot{width:10px;height:10px;border-radius:999px;background:var(--accent); box-shadow: 0 0 18px rgba(44,255,143,.45)}  
    header{  
      position:sticky; top:0; z-index:20;  
      background: linear-gradient(to bottom, rgba(11,11,11,.92), rgba(11,11,11,.65), transparent);  
      backdrop-filter: blur(10px);  
      border-bottom: 1px solid rgba(255,255,255,.06);  
    }  
    .nav{  
      display:flex; align-items:center; justify-content:space-between;  
      gap:16px;  
      padding:14px 24px;  
      max-width:var(--max);  
      margin:0 auto;  
    }  
    .brand{  
      display:flex; align-items:center; gap:12px;  
      font-weight:800;  
      letter-spacing:.6px;  
      text-transform:uppercase;  
    }  
    .brand small{  
      display:block;  
      font-weight:600;  
      letter-spacing:.2px;  
      color:var(--muted);  
      text-transform:none;  
      margin-top:2px;  
    }  
    .navlinks{display:flex; align-items:center; gap:14px}  
    .navlinks a{  
      padding:10px 12px;  
      border-radius:999px;  
      color:var(--muted);  
      transition:.2s ease;  
    }  
    .navlinks a:hover{color:var(--text); background: rgba(255,255,255,.06)}  
    .cta{  
      display:inline-flex; align-items:center; justify-content:center; gap:10px;  
      padding:10px 14px;  
      border-radius:999px;  
      border:1px solid rgba(44,255,143,.35);  
      background: rgba(44,255,143,.10);  
      color: var(--text);  
      box-shadow: 0 0 0 0 rgba(44,255,143,.0);  
      transition: .2s ease;  
      white-space:nowrap;  
    }  
    .cta:hover{background: rgba(44,255,143,.16); box-shadow: 0 0 0 6px rgba(44,255,143,.08)}  
    .hero{  
      padding:46px 0 22px;  
    }  
    .hero-grid{  
      display:grid;  
      grid-template-columns: 1.1fr .9fr;  
      gap:22px;  
      align-items:stretch;  
    }  
    .h1{  
      font-size: clamp(34px, 5vw, 64px);  
      line-height:1.02;  
      letter-spacing:-.8px;  
      margin:12px 0 14px;  
      font-weight:900;  
      text-transform:uppercase;  
    }  
    .sub{  
      color:var(--muted);  
      font-size: 16px;  
      max-width: 60ch;  
    }  
    .hero-card{  
      border:1px solid rgba(255,255,255,.10);  
      border-radius: var(--radius2);  
      background: linear-gradient(180deg, rgba(255,255,255,.05), rgba(255,255,255,.02));  
      box-shadow: var(--shadow);  
      overflow:hidden;  
      position:relative;  
    }  
    .hero-card .pad{padding:18px}  
    .badge{  
      display:inline-flex; align-items:center; gap:10px;  
      padding:10px 12px;  
      border-radius:999px;  
      border:1px solid rgba(255,255,255,.12);  
      background: rgba(0,0,0,.25);  
      color:var(--muted);  
      font-weight:600;  
      width:fit-content;  
    }  
    .grid-mini{  
      display:grid;  
      grid-template-columns:1fr 1fr;  
      gap:12px;  
      padding:18px;  
    }  
    .mini{  
      border:1px solid rgba(255,255,255,.10);  
      border-radius:16px;  
      padding:14px;  
      background: rgba(0,0,0,.18);  
    }  
    .mini b{display:block; margin-bottom:6px}  
    .mini span{color:var(--muted); font-size:13px}  
    .bar{  
      height:1px;  
      background: rgba(255,255,255,.08);  
      margin: 18px 0;  
    }  
  
    section{padding:22px 0}  
    .section-title{  
      display:flex; align-items:flex-end; justify-content:space-between; gap:12px;  
      margin: 10px 0 12px;  
    }  
    .section-title h2{  
      margin:0;  
      font-size: 22px;  
      letter-spacing:-.2px;  
      text-transform:uppercase;  
    }  
    .section-title p{margin:0;color:var(--muted); font-size:14px}  
  
    .products{  
      display:grid;  
      grid-template-columns: repeat(3, 1fr);  
      gap:14px;  
    }  
    .card{  
      border:1px solid rgba(255,255,255,.10);  
      border-radius: var(--radius);  
      background: rgba(255,255,255,.03);  
      overflow:hidden;  
      box-shadow: 0 10px 26px rgba(0,0,0,.25);  
      transition: .18s ease;  
      min-height: 320px;  
      display:flex; flex-direction:column;  
    }  
    .card:hover{transform: translateY(-3px); border-color: rgba(44,255,143,.35)}  
    .img{  
      height: 150px;  
      background:  
        radial-gradient(500px 240px at 20% 20%, rgba(44,255,143,.22), transparent 55%),  
        linear-gradient(135deg, rgba(255,255,255,.08), rgba(255,255,255,.02));  
      border-bottom: 1px solid rgba(255,255,255,.10);  
      position:relative;  
    }  
    .img::after{  
      content:"GC";  
      position:absolute; right:14px; bottom:12px;  
      font-weight:900; letter-spacing:2px;  
      color: rgba(255,255,255,.18);  
      font-size: 28px;  
      text-transform:uppercase;  
    }  
    .card .content{padding:14px; display:flex; flex-direction:column; gap:10px; flex:1}  
    .card h3{margin:0; font-size:16px; text-transform:uppercase; letter-spacing:.4px}  
    .desc{margin:0; color:var(--muted); font-size:14px}  
    .row{display:flex; gap:10px; flex-wrap:wrap; align-items:center}  
    .chip{  
      display:inline-flex; align-items:center; gap:8px;  
      padding:8px 10px;  
      border-radius:999px;  
      border:1px solid rgba(255,255,255,.12);  
      background: rgba(0,0,0,.25);  
      color:var(--muted);  
      font-size:13px;  
    }  
    .swatch{  
      width:10px;height:10px;border-radius:999px;  
      border:1px solid rgba(255,255,255,.22);  
      background:#fff;  
    }  
    .swatch.black{background:#0b0b0b}  
    .swatch.white{background:#f5f5f5}  
    .swatch.green{background:var(--accent)}  
    .swatch.grey{background:#8a8a8a}  
    .swatch.lightwash{background:#bcd0ff}  
    .swatch.darkwash{background:#3e5b8a}  
  
    .actions{margin-top:auto; display:flex; gap:10px}  
    .btn{  
      flex:1;  
      display:inline-flex; align-items:center; justify-content:center; gap:10px;  
      padding:10px 12px;  
      border-radius:12px;  
      border:1px solid rgba(255,255,255,.12);  
      background: rgba(255,255,255,.04);  
      color: var(--text);  
      font-weight:700;  
      transition:.18s ease;  
    }  
    .btn:hover{background: rgba(255,255,255,.07)}  
    .btn.primary{  
      border-color: rgba(44,255,143,.35);  
      background: rgba(44,255,143,.10);  
    }  
    .btn.primary:hover{background: rgba(44,255,143,.16)}  
    .about{  
      display:grid;  
      grid-template-columns: 1fr 1fr;  
      gap:14px;  
    }  
    .panel{  
      border:1px solid rgba(255,255,255,.10);  
      border-radius: var(--radius);  
      background: rgba(255,255,255,.03);  
      padding:16px;  
    }  
    .panel h3{margin:0 0 8px; text-transform:uppercase; letter-spacing:.4px}  
    .panel p{margin:0; color:var(--muted)}  
    .signup{  
      display:flex; gap:10px; margin-top:12px; flex-wrap:wrap;  
    }  
    input{  
      flex:1;  
      min-width: 220px;  
      padding:12px 12px;  
      border-radius:12px;  
      border:1px solid rgba(255,255,255,.12);  
      background: rgba(0,0,0,.30);  
      color:var(--text);  
      outline:none;  
    }  
    input:focus{border-color: rgba(44,255,143,.5); box-shadow: 0 0 0 6px rgba(44,255,143,.08)}  
    footer{  
      padding:26px 0 34px;  
      color: var(--muted);  
      border-top: 1px solid rgba(255,255,255,.08);  
      margin-top: 18px;  
    }  
  
    /* responsive */  
    @media (max-width: 920px){  
      .hero-grid{grid-template-columns:1fr}  
      .products{grid-template-columns:1fr}  
      .about{grid-template-columns:1fr}  
      .navlinks{display:none}  
    }  
  </style>  
</head>  
  
<body>  
  <header>  
    <div class="nav">  
      <a class="brand" href="#top" aria-label="Gents Collective home">  
        <span style="display:inline-flex;align-items:center;gap:10px">  
          <span class="dot" aria-hidden="true"></span>  
          <span>Gents Collective</span>  
        </span>  
        <small>Streetwear • Simple • Clean</small>  
      </a>  
  
      <nav class="navlinks" aria-label="Primary">  
        <a href="#drops">Drops</a>  
        <a href="#products">Products</a>  
        <a href="#about">About</a>  
      </nav>  
  
      <a class="cta" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">  
        Follow @Brentgocraze →  
      </a>  
    </div>  
  </header>  
  
  <main id="top" class="wrap">  
    <section class="hero">  
      <div class="pill" aria-label="Brand tagline">  
        <span class="dot" aria-hidden="true"></span>  
        <span style="color:var(--muted);font-weight:600">Modern monochrome streetwear with a clean silhouette.</span>  
      </div>  
  
      <div class="hero-grid" style="margin-top:14px">  
        <div>  
          <h1 class="h1">Gents<br/>Collective</h1>  
          <p class="sub">  
            Oversized essentials built for everyday rotation — minimal, neat, and bold.  
            Shop the core pieces below and tap in on Instagram for drops.  
          </p>  
  
          <div class="bar"></div>  
  
          <div class="row">  
            <a class="btn primary" href="#products">Shop Core Pieces</a>  
            <a class="btn" href="#drops">Get Drop Updates</a>  
          </div>  
  
          <p class="sub" style="margin-top:12px">  
            Color system: <span style="color:var(--text);font-weight:700">Black / White</span>  
            with a <span style="color:var(--accent);font-weight:800">Modern Green</span> accent.  
          </p>  
        </div>  
  
        <div class="hero-card" aria-label="Quick brand highlights">  
          <div class="pad">  
            <div class="badge">Core Line • 3 Essentials • Clean Fit</div>  
          </div>  
          <div class="grid-mini">  
            <div class="mini">  
              <b>Oversized Tee</b>  
              <span>Black • White • Green</span>  
            </div>  
            <div class="mini">  
              <b>Baggy Jeans</b>  
              <span>Light Wash • Dark Wash • Black</span>  
            </div>  
            <div class="mini">  
              <b>Heavy Hoodie</b>  
              <span>Black • Grey • White</span>  
            </div>  
            <div class="mini">  
              <b>Drop Ready</b>  
              <span>Link to purchase + IG updates</span>  
            </div>  
          </div>  
        </div>  
      </div>  
    </section>  
  
    <section id="products">  
      <div class="section-title">  
        <h2>Core Pieces</h2>  
        <p>Clean layouts • Simple choices • Easy to shop</p>  
      </div>  
  
      <div class="products">  
        <!-- Oversized Tee -->  
        <article class="card">  
          <div class="img" aria-hidden="true"></div>  
          <div class="content">  
            <h3>Oversized Tee</h3>  
            <p class="desc">Relaxed drape. Minimal branding. Built for a clean streetwear fit.</p>  
  
            <div class="row" aria-label="Tee colors">  
              <span class="chip"><span class="swatch black"></span> Black</span>  
              <span class="chip"><span class="swatch white"></span> White</span>  
              <span class="chip"><span class="swatch green"></span> Green</span>  
            </div>  
  
            <div class="actions">  
              <a class="btn primary" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">Buy / DM</a>  
              <a class="btn" href="#drops">Notify Me</a>  
            </div>  
          </div>  
        </article>  
  
        <!-- Baggy Jeans -->  
        <article class="card">  
          <div class="img" aria-hidden="true"></div>  
          <div class="content">  
            <h3>Baggy Jeans</h3>  
            <p class="desc">Loose leg. Everyday wear. Matches oversized tops perfectly.</p>  
  
            <div class="row" aria-label="Jean colors">  
              <span class="chip"><span class="swatch lightwash"></span> Light Wash</span>  
              <span class="chip"><span class="swatch darkwash"></span> Dark Wash</span>  
              <span class="chip"><span class="swatch black"></span> Black</span>  
            </div>  
  
            <div class="actions">  
              <a class="btn primary" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">Buy / DM</a>  
              <a class="btn" href="#drops">Notify Me</a>  
            </div>  
          </div>  
        </article>  
  
        <!-- Heavy Oversized Hoodie -->  
        <article class="card">  
          <div class="img" aria-hidden="true"></div>  
          <div class="content">  
            <h3>Heavy Oversized Hoodie</h3>  
            <p class="desc">Thick, structured feel with a clean oversized silhouette.</p>  
  
            <div class="row" aria-label="Hoodie colors">  
              <span class="chip"><span class="swatch black"></span> Black</span>  
              <span class="chip"><span class="swatch grey"></span> Grey</span>  
              <span class="chip"><span class="swatch white"></span> White</span>  
            </div>  
  
            <div class="actions">  
              <a class="btn primary" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">Buy / DM</a>  
              <a class="btn" href="#drops">Notify Me</a>  
            </div>  
          </div>  
        </article>  
      </div>  
    </section>  
  
    <section id="drops">  
      <div class="section-title">  
        <h2>Drop Updates</h2>  
        <p>Collect emails or send people straight to IG</p>  
      </div>  
  
      <div class="about">  
        <div class="panel">  
          <h3>Get Notified</h3>  
          <p>  
            Add your email list here (free). For now, this form is set up as a placeholder.  
            If you want, I can wire it to a free email tool (like Mailchimp) later.  
          </p>  
  
          <form class="signup" onsubmit="event.preventDefault(); alert('Saved! (Demo)');">  
            <input type="email" placeholder="Email address" required />  
            <button class="btn primary" type="submit">Join List</button>  
          </form>  
  
          <p style="margin-top:10px;color:var(--muted);font-size:13px">  
            Tip: For early drops, use “IG DM to order” and later switch to a checkout link.  
          </p>  
        </div>  
  
        <div class="panel">  
          <h3>Order Method</h3>  
          <p>  
            Right now your “Buy / DM” buttons send customers to Instagram:  
            <b style="color:var(--text)">@Brentgocraze</b>. Perfect for early stage (simple + fast).  
          </p>  
          <div class="bar"></div>  
          <div class="row">  
            <a class="btn primary" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">Open Instagram</a>  
            <a class="btn" href="#about">Brand Story</a>  
          </div>  
        </div>  
      </div>  
    </section>  
  
    <section id="about">  
      <div class="section-title">  
        <h2>About</h2>  
        <p>Minimal. Clean. Neat. Streetwear essentials.</p>  
      </div>  
  
      <div class="panel">  
        <h3>Gents Collective</h3>  
        <p>  
          Built around clean silhouettes and simple colorways — black, white, and modern green.  
          Oversized tees, baggy jeans, and heavy hoodies designed to look sharp with zero effort.  
        </p>  
      </div>  
    </section>  
  
    <footer>  
      <div class="wrap" style="padding:0">  
        <div style="display:flex; flex-wrap:wrap; gap:10px; align-items:center; justify-content:space-between">  
          <div>© <span id="y"></span> Gents Collective</div>  
          <div class="row">  
            <a class="pill" href="https://instagram.com/Brentgocraze" target="_blank" rel="noopener">  
              <span class="dot" aria-hidden="true"></span>  
              <span>@Brentgocraze</span>  
            </a>  
            <a class="pill" href="#top">Back to top ↑</a>  
          </div>  
        </div>  
      </div>  
    </footer>  
  </main>  
  
  <script>  
    document.getElementById("y").textContent = new Date().getFullYear();  
  </script>  
</body>  
</html>  
