<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ivan Kovalyshyn — Editing · Scripts · Thumbnails</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Space+Mono:wght@400;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #0E0D0F;
    --panel: #17161A;
    --panel-2: #1E1C21;
    --hairline: #2E2C31;
    --text: #F1EDE6;
    --text-dim: #948F8A;
    --video: #E8823D;
    --video-dim: #4A3323;
    --audio: #6FA88C;
    --audio-dim: #253430;
    --fx: #C9A6E8;
    --fx-dim: #322A3B;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--bg);
    color:var(--text);
    font-family:'Inter',sans-serif;
    line-height:1.6;
    overflow-x:hidden;
  }
  ::selection{background:var(--video);color:#0E0D0F;}
  a{color:inherit;}
  .mono{font-family:'Space Mono',monospace;}
  .display{font-family:'Bebas Neue',sans-serif;letter-spacing:0.02em;}

  /* subtle grain texture */
  body::before{
    content:"";
    position:fixed;inset:0;
    pointer-events:none;
    z-index:999;
    opacity:0.035;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
  }

  /* ---------- SCRUBBER (sticky timeline nav) ---------- */
  .scrubber{
    position:sticky;top:0;z-index:100;
    background:rgba(14,13,15,0.92);
    backdrop-filter:blur(8px);
    border-bottom:1px solid var(--hairline);
  }
  .scrubber-track{
    position:relative;
    height:3px;
    background:var(--hairline);
  }
  .scrubber-fill{
    position:absolute;left:0;top:0;height:100%;
    width:0%;
    background:var(--video);
    transition:width 0.1s linear;
  }
  .scrubber-marks{
    display:flex;
    justify-content:space-between;
    max-width:1100px;
    margin:0 auto;
    padding:10px 24px;
    gap:8px;
  }
  .scrubber-marks a{
    text-decoration:none;
    font-size:11px;
    letter-spacing:0.05em;
    color:var(--text-dim);
    white-space:nowrap;
    display:flex;
    flex-direction:column;
    align-items:center;
    gap:2px;
    transition:color 0.2s;
  }
  .scrubber-marks a:hover, .scrubber-marks a.active{color:var(--video);}
  .scrubber-marks .tick{
    width:1px;height:6px;background:var(--hairline);
  }
  .scrubber-marks a.active .tick{background:var(--video);}
  @media (max-width:640px){
    .scrubber-marks a span.label{display:none;}
    .scrubber-marks{padding:8px 16px;}
  }

  section{
    max-width:1100px;
    margin:0 auto;
    padding:110px 24px;
  }
  .eyebrow{
    font-size:12px;
    color:var(--video);
    text-transform:uppercase;
    letter-spacing:0.15em;
    margin-bottom:14px;
    display:flex;
    align-items:center;
    gap:10px;
  }
  .eyebrow::before{
    content:"";
    width:14px;height:14px;
    border:1.5px solid var(--video);
    border-radius:50%;
    position:relative;
  }
  .eyebrow::after{
    content:"";
    position:absolute;
    width:5px;height:5px;
    background:var(--video);
    border-radius:50%;
    margin-left:-9.5px;
  }

  /* ---------- HERO ---------- */
  .hero{
    padding-top:70px;
    min-height:86vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
  }
  .hero-tc{
    font-size:13px;color:var(--text-dim);
    margin-bottom:20px;
  }
  h1.name{
    font-size:clamp(3.2rem, 10vw, 7.5rem);
    line-height:0.92;
    text-transform:uppercase;
  }
  .roles{
    margin-top:26px;
    display:flex;
    flex-wrap:wrap;
    gap:10px;
  }
  .role-chip{
    font-size:13px;
    padding:6px 14px;
    border:1px solid var(--hairline);
    border-radius:3px;
    color:var(--text-dim);
    background:var(--panel);
  }
  .hero-note{
    margin-top:40px;
    max-width:520px;
    color:var(--text-dim);
    font-size:15px;
    border-left:2px solid var(--video);
    padding-left:16px;
  }

  /* ---------- ABOUT ---------- */
  .about-grid{
    display:grid;
    grid-template-columns:120px 1fr;
    gap:40px;
  }
  .logline-tag{
    font-size:12px;color:var(--text-dim);
    writing-mode:vertical-rl;
    text-orientation:mixed;
    letter-spacing:0.1em;
  }
  .about-panel{
    background:var(--panel);
    border:1px solid var(--hairline);
    border-radius:4px;
    padding:36px;
  }
  .about-panel p{font-size:17px;color:#DAD5CD;max-width:620px;}
  .about-panel p + p{margin-top:14px;}
  @media (max-width:640px){
    .about-grid{grid-template-columns:1fr;}
    .logline-tag{writing-mode:horizontal-tb;}
  }

  /* ---------- WORK / REELS ---------- */
  .reel{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:0;
    border:1px solid var(--hairline);
    border-radius:4px;
    overflow:hidden;
    margin-bottom:24px;
    background:var(--panel);
  }
  .reel-info{padding:36px;display:flex;flex-direction:column;justify-content:center;}
  .reel-num{font-size:13px;color:var(--video);margin-bottom:10px;}
  .reel-title{font-size:1.6rem;font-weight:700;margin-bottom:10px;}
  .reel-desc{color:var(--text-dim);font-size:14.5px;margin-bottom:22px;}
  .reel-visual{
    background:
      repeating-linear-gradient(135deg, var(--panel-2) 0 2px, transparent 2px 14px);
    position:relative;
    display:flex;align-items:center;justify-content:center;
    min-height:180px;
    border-left:1px solid var(--hairline);
  }
  .play-btn{
    width:60px;height:60px;border-radius:50%;
    border:1.5px solid var(--video);
    display:flex;align-items:center;justify-content:center;
    transition:transform 0.25s, background 0.25s;
  }
  .reel:hover .play-btn{background:var(--video);transform:scale(1.08);}
  .play-btn svg{fill:var(--video);transition:fill 0.25s;}
  .reel:hover .play-btn svg{fill:#0E0D0F;}
  .btn{
    display:inline-flex;align-items:center;gap:8px;
    align-self:flex-start;
    font-size:13px;font-weight:600;
    padding:11px 20px;
    border:1px solid var(--video);
    color:var(--video);
    border-radius:3px;
    text-decoration:none;
    transition:background 0.2s, color 0.2s;
  }
  .btn:hover{background:var(--video);color:#0E0D0F;}
  .status-badge{
    font-size:11px;
    padding:3px 9px;
    border-radius:10px;
    display:inline-block;
    margin-bottom:14px;
    width:fit-content;
  }
  .status-open{background:var(--audio-dim);color:var(--audio);}
  .status-closed{background:var(--fx-dim);color:var(--fx);}
  @media (max-width:720px){
    .reel{grid-template-columns:1fr;}
    .reel-visual{min-height:120px;border-left:none;border-top:1px solid var(--hairline);}
  }

  /* ---------- SKILLS TIMELINE ---------- */
  .timeline-tracks{
    border:1px solid var(--hairline);
    border-radius:4px;
    overflow:hidden;
  }
  .track{
    display:grid;
    grid-template-columns:140px 1fr;
    border-bottom:1px solid var(--hairline);
  }
  .track:last-child{border-bottom:none;}
  .track-label{
    padding:22px 16px;
    font-size:12px;
    color:var(--text-dim);
    background:var(--panel);
    border-right:1px solid var(--hairline);
    display:flex;
    flex-direction:column;
    justify-content:center;
    gap:2px;
  }
  .track-label b{color:var(--text);font-size:13px;}
  .track-lane{
    position:relative;
    padding:18px 20px;
    background:
      repeating-linear-gradient(90deg, transparent 0 79px, var(--hairline) 79px 80px);
    display:flex;align-items:center;
  }
  .clip{
    padding:10px 18px;
    border-radius:3px;
    font-size:14px;
    font-weight:500;
  }
  .clip-video{background:var(--video-dim);color:var(--video);border:1px solid var(--video);}
  .clip-audio{background:var(--audio-dim);color:var(--audio);border:1px solid var(--audio);}
  .clip-fx{background:var(--fx-dim);color:var(--fx);border:1px solid var(--fx);}
  @media (max-width:640px){
    .track{grid-template-columns:100px 1fr;}
    .track-label{padding:16px 10px;}
  }

  /* ---------- CONTACT / END CARD ---------- */
  .endcard{
    border:1px solid var(--hairline);
    border-radius:4px;
    padding:60px 40px;
    text-align:center;
    background:radial-gradient(circle at 50% 0%, var(--panel-2), var(--panel));
  }
  .rec-badge{
    display:inline-flex;align-items:center;gap:8px;
    font-size:12px;letter-spacing:0.08em;
    color:var(--audio);
    border:1px solid var(--audio);
    padding:6px 14px;border-radius:20px;
    margin-bottom:28px;
  }
  .rec-dot{
    width:8px;height:8px;border-radius:50%;
    background:#FF5C4D;
    animation:pulse 1.6s infinite;
  }
  @keyframes pulse{
    0%,100%{opacity:1;}
    50%{opacity:0.25;}
  }
  @media (prefers-reduced-motion: reduce){
    .rec-dot{animation:none;}
    html{scroll-behavior:auto;}
  }
  .endcard h2{
    font-family:'Bebas Neue',sans-serif;
    font-size:clamp(2.4rem,6vw,4rem);
    text-transform:uppercase;
    margin-bottom:18px;
  }
  .endcard p{color:var(--text-dim);max-width:480px;margin:0 auto 34px;}
  .contact-links{display:flex;gap:16px;justify-content:center;flex-wrap:wrap;}
  .contact-links a{
    padding:14px 26px;
    border:1px solid var(--hairline);
    border-radius:4px;
    text-decoration:none;
    font-size:14px;font-weight:600;
    display:flex;align-items:center;gap:10px;
    transition:border-color 0.2s, transform 0.2s;
  }
  .contact-links a:hover{border-color:var(--video);transform:translateY(-2px);}

  footer{
    text-align:center;
    padding:30px 24px 50px;
    font-size:12px;
    color:var(--text-dim);
  }
</style>
</head>
<body>

<div class="scrubber">
  <div class="scrubber-marks mono">
    <a href="#intro" class="active" data-target="intro"><span class="label">00:00 INTRO</span><span class="tick"></span></a>
    <a href="#about" data-target="about"><span class="label">00:12 ABOUT</span><span class="tick"></span></a>
    <a href="#work" data-target="work"><span class="label">00:24 REELS</span><span class="tick"></span></a>
    <a href="#skills" data-target="skills"><span class="label">00:40 SKILLS</span><span class="tick"></span></a>
    <a href="#contact" data-target="contact"><span class="label">00:55 CONTACT</span><span class="tick"></span></a>

  </div>
  <div class="scrubber-track"><div class="scrubber-fill" id="scrubFill"></div></div>
</div>

<section class="hero" id="intro">
  <div class="hero-tc mono">REEL // 00:00:00:00 — TAKE 1</div>
  <h1 class="display name">Ivan<br>Kovalyshyn</h1>
  <div class="roles mono">
    <span class="role-chip">Video Editing</span>
    <span class="role-chip">Scriptwriting</span>
    <span class="role-chip">Thumbnail Design</span>
    <span class="role-chip">AI-Hybrid Workflow</span>
  </div>
  <p class="hero-note">I make videos from script to final render on my own — by hand where the details matter, and with AI where it genuinely speeds things up.</p>
</section>

<section id="about">
  <div class="eyebrow mono">Scene 01 — Logline</div>
  <div class="about-grid">
    <div class="logline-tag mono">ABOUT / IVAN K.</div>
    <div class="about-panel">
      <p>Student, self-taught. I handle every project myself — no team, no outsourcing: from the idea and script to the edit and the cover.</p>
      <p>I blend classic editing with AI tools wherever it's justified — faster, without losing image quality or rhythm.</p>
      <p>Currently open for freelance work in this niche — editing, scripts, and thumbnails for YouTube.</p>
    </div>
  </div>
</section>

<section id="work">
  <div class="eyebrow mono">Scene 02 — Reels</div>

  <div class="reel">
    <div class="reel-info">
      <div class="reel-num mono">REEL 01</div>
      <span class="status-badge status-open">PUBLIC CHANNEL</span>
      <div class="reel-title">101ds-edits</div>
      <div class="reel-desc">Public editing work — open for anyone to watch.</div>
      <a class="btn" href="https://www.youtube.com/@101ds-edits" target="_blank" rel="noopener">
        Watch on YouTube →
      </a>
    </div>
    <div class="reel-visual">
      <div class="play-btn"><svg width="20" height="20" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg></div>
    </div>
  </div>

  <div class="reel">
    <div class="reel-info">
      <div class="reel-num mono">REEL 02</div>
      <span class="status-badge status-closed">PRIVATE CHANNEL</span>
      <div class="reel-title">object_ua</div>
      <div class="reel-desc">Client / private project — access on request.</div>
      <a class="btn" href="https://www.youtube.com/@object_ua" target="_blank" rel="noopener">
        Visit Channel →
      </a>
    </div>
    <div class="reel-visual">
      <div class="play-btn"><svg width="20" height="20" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg></div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="eyebrow mono">Scene 03 — Tracks</div>
  <div class="timeline-tracks mono">
    <div class="track">
      <div class="track-label">V2 <b>GFX</b></div>
      <div class="track-lane"><div class="clip clip-video">Thumbnails & covers for YouTube</div></div>
    </div>
    <div class="track">
      <div class="track-label">V1 <b>EDIT</b></div>
      <div class="track-lane"><div class="clip clip-video">Video editing, pacing, cuts</div></div>
    </div>
    <div class="track">
      <div class="track-label">A1 <b>SCRIPT</b></div>
      <div class="track-lane"><div class="clip clip-audio">Scripts, structure, hooks</div></div>
    </div>
    <div class="track">
      <div class="track-label">FX <b>AI</b></div>
      <div class="track-lane"><div class="clip clip-fx">Hybrid workflow with AI tools</div></div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="eyebrow mono">Final</div>
  <div class="endcard">
    <div class="rec-badge mono"><span class="rec-dot"></span>REC — Open for freelance work</div>
    <h2 class="display">Got a project?<br>Let's talk.</h2>
    <p>Editing, scripts, or thumbnails for your channel — let's discuss the details and timeline.</p>
    <div class="contact-links mono">
      <a href="mailto:motivationup7797@gmail.com">✉ Email</a>
      <a href="https://t.me/objy007" target="_blank" rel="noopener">✈ Telegram</a>
    </div>
  </div>
</section>

<footer class="mono">© Ivan Kovalyshyn — Video Editing / Scriptwriting / Thumbnails</footer>

<script>
  // Scrollspy + scrubber fill
  const sections = ['intro','about','work','skills','contact'].map(id => document.getElementById(id));
  const links = document.querySelectorAll('.scrubber-marks a');
  const fill = document.getElementById('scrubFill');

  function onScroll(){
    const scrollTop = window.scrollY;
    const docHeight = document.documentElement.scrollHeight - window.innerHeight;
    const pct = docHeight > 0 ? (scrollTop / docHeight) * 100 : 0;
    fill.style.width = pct + '%';

    let current = sections[0].id;
    for(const s of sections){
      const rect = s.getBoundingClientRect();
      if(rect.top <= window.innerHeight * 0.4){
        current = s.id;
      }
    }
    links.forEach(a => a.classList.toggle('active', a.dataset.target === current));
  }
  window.addEventListener('scroll', onScroll, {passive:true});
  onScroll();
</script>

</body>
</html>
