<!doctype html>  
<html lang="en">  
<head>  
  <meta charset="utf-8" />  
  <meta name="viewport" content="width=device-width, initial-scale=1" />  
  <title>Heru 💌</title>  
  <style>  
    :root{  
      --bg1:#0b0b14;  
      --bg2:#1a1030;  
      --card:#ffffff0f;  
      --text:#f7f2ff;  
      --muted:#cbb9ff;  
      --accent:#ff5bbd;  
      --accent2:#7c5cff;  
      --good:#34d399;  
    }  
    *{box-sizing:border-box}  
    body{  
      margin:0;  
      min-height:100vh;  
      display:flex;  
      align-items:center;  
      justify-content:center;  
      color:var(--text);  
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;  
      background:  
        radial-gradient(1000px 600px at 20% 20%, #ff5bbd22, transparent 60%),  
        radial-gradient(900px 500px at 80% 30%, #7c5cff22, transparent 55%),  
        linear-gradient(135deg, var(--bg1), var(--bg2));  
      overflow:hidden;  
    }  
    .card{  
      width:min(720px, 92vw);  
      padding:28px 22px;  
      border:1px solid #ffffff1f;  
      border-radius:20px;  
      background:linear-gradient(180deg, #ffffff14, #ffffff08);  
      box-shadow: 0 20px 80px #00000055;  
      position:relative;  
    }  
    .top{  
      display:flex;  
      gap:14px;  
      align-items:center;  
      justify-content:center;  
      margin-bottom:10px;  
      flex-wrap:wrap;  
    }  
    .pill{  
      font-size:13px;  
      padding:7px 12px;  
      border-radius:999px;  
      border:1px solid #ffffff22;  
      background:#00000020;  
      color:var(--muted);  
      letter-spacing:.2px;  
    }  
    h1{  
      font-size: clamp(30px, 6vw, 52px);  
      margin:10px 0 6px;  
      text-align:center;  
      line-height:1.05;  
    }  
    .sub{  
      text-align:center;  
      color:var(--muted);  
      font-size:16px;  
      margin:0 0 18px;  
    }  
    .message{  
      text-align:center;  
      font-size:17px;  
      line-height:1.5;  
      color:#f1eaff;  
      margin: 0 auto 22px;  
      max-width: 58ch;  
    }  
    .highlight{  
      color:var(--accent);  
      font-weight:700;  
    }  
    .buttons{  
      display:flex;  
      gap:12px;  
      justify-content:center;  
      flex-wrap:wrap;  
      margin-top:10px;  
    }  
    button{  
      border:none;  
      border-radius:14px;  
      padding:12px 18px;  
      font-size:16px;  
      cursor:pointer;  
      transition: transform .08s ease, filter .12s ease;  
      user-select:none;  
    }  
    button:active{transform: translateY(1px) scale(.99)}  
    .yes{  
      background: linear-gradient(135deg, var(--accent), var(--accent2));  
      color:white;  
      box-shadow: 0 12px 30px #ff5bbd33;  
      min-width:140px;  
    }  
    .no{  
      background:#ffffff12;  
      color:#ffffffcc;  
      border:1px solid #ffffff22;  
      min-width:140px;  
      position:relative;  
    }  
    .footer{  
      text-align:center;  
      margin-top:18px;  
      font-size:13px;  
      color:#ffffff9a;  
    }  
    .tiny{  
      font-size:12px;  
      color:#ffffff80;  
      text-align:center;  
      margin-top:6px;  
    }  
    .sparkle{  
      position:absolute;  
      inset:-2px;  
      border-radius:22px;  
      pointer-events:none;  
      background:  
        radial-gradient(350px 120px at 20% 10%, #ff5bbd25, transparent 60%),  
        radial-gradient(260px 100px at 80% 0%, #7c5cff22, transparent 55%);  
      filter: blur(10px);  
      opacity:.9;  
    }  
  
    /* Floating hearts */  
    .heart{  
      position:absolute;  
      width:16px;  
      height:16px;  
      transform: rotate(45deg);  
      background: var(--accent);  
      opacity:.65;  
      animation: floatUp linear forwards;  
      border-radius:3px;  
    }  
    .heart::before,.heart::after{  
      content:"";  
      position:absolute;  
      width:16px;height:16px;  
      background: inherit;  
      border-radius:50%;  
    }  
    .heart::before{left:-8px; top:0}  
    .heart::after{left:0; top:-8px}  
  
    @keyframes floatUp{  
      from{ transform: translateY(0) rotate(45deg); }  
      to{ transform: translateY(-120vh) rotate(45deg); }  
    }  
  
    /* Success screen */  
    .success{  
      display:none;  
      text-align:center;  
      padding:10px 0 0;  
    }  
    .success h2{  
      margin:10px 0 6px;  
      font-size: clamp(26px, 5vw, 40px);  
      color: #d9ffe9;  
    }  
    .success p{  
      margin:0 auto;  
      max-width: 60ch;  
      color:#c8ffe0;  
      line-height:1.5;  
      font-size:16px;  
    }  
    .ok{  
      margin-top:16px;  
      background: #ffffff12;  
      border:1px solid #ffffff22;  
      color:#ffffffd0;  
      padding:10px 14px;  
      border-radius:12px;  
      cursor:pointer;  
    }  
  </style>  
</head>  
<body>  
  <div class="card" id="card">  
    <div class="sparkle"></div>  
  
    <div id="main">  
      <div class="top">  
        <div class="pill">From: <span class="highlight">Your man</span></div>  
        <div class="pill">To: <span class="highlight">Heru</span></div>  
      </div>  
  
      <h1>Heru… 💘</h1>  
      <p class="sub">Quick question, no pressure… but also kinda pressure 😭</p>  
  
      <p class="message">  
        I just wanted to say you’ve been on my mind a lot.  
        Your vibe is different in the best way, and I’d be lying if I said I didn’t want to make  
        <span class="highlight">Valentine’s</span> feel special this year.  
        <br><br>  
        Sooo… will you be <span class="highlight">my Valentine</span>? 🌹  
      </p>  
  
      <div class="buttons">  
        <button class="yes" id="yesBtn">Yes 😁💗</button>  
        <button class="no" id="noBtn">No 🙃</button>  
      </div>  
  
      <div class="footer">If you press “Yes” I’m basically doing a happy dance.</div>  
      <div class="tiny">(You can still say no. I’ll survive. Probably.)</div>  
    </div>  
  
    <div class="success" id="success">  
      <h2>WOOOO 😭💚</h2>  
      <p>  
        Okay bet. That just made my whole day.  
        <br>  
        Now we gotta celebrate properly… date idea loading… 🍓🎬🌆  
      </p>  
      <button class="ok" id="okBtn">Replay the hearts ✨</button>  
    </div>  
  </div>  
  
  <script>  
    const yesBtn = document.getElementById("yesBtn");  
    const noBtn = document.getElementById("noBtn");  
    const main = document.getElementById("main");  
    const success = document.getElementById("success");  
    const okBtn = document.getElementById("okBtn");  
  
    // Spawn floating hearts  
    function spawnHearts(count = 18){  
      for(let i=0;i<count;i++){  
        const h = document.createElement("div");  
        h.className = "heart";  
        const size = 10 + Math.random()*18;  
        h.style.width = size + "px";  
        h.style.height = size + "px";  
        h.style.left = (Math.random()*100) + "vw";  
        h.style.bottom = (-20 - Math.random()*40) + "px";  
        h.style.opacity = (0.35 + Math.random()*0.55).toFixed(2);  
  
        const duration = 4 + Math.random()*4;  
        h.style.animationDuration = duration + "s";  
  
        // Slight color shift  
        const hue = 320 + Math.random()*40; // pink-ish  
        h.style.background = `hsl(${hue} 100% 70%)`;  
  
        document.body.appendChild(h);  
        setTimeout(()=> h.remove(), duration*1000);  
      }  
    }  
  
    yesBtn.addEventListener("click", () => {  
      spawnHearts(35);  
      main.style.display = "none";  
      success.style.display = "block";  
    });  
  
    // No button playfully dodges the cursor/tap  
    function dodge(){  
      const rect = noBtn.getBoundingClientRect();  
      const pad = 14;  
      const maxX = window.innerWidth - rect.width - pad;  
      const maxY = window.innerHeight - rect.height - pad;  
  
      // random position but keep it on screen  
      const x = Math.max(pad, Math.min(maxX, Math.random()*maxX));  
      const y = Math.max(pad, Math.min(maxY, Math.random()*maxY));  
  
      noBtn.style.position = "fixed";  
      noBtn.style.left = x + "px";  
      noBtn.style.top = y + "px";  
    }  
  
    noBtn.addEventListener("mouseenter", dodge);  
    noBtn.addEventListener("click", dodge); // for mobile taps  
  
    okBtn.addEventListener("click", () => spawnHearts(30));  
  
    // subtle background hearts occasionally  
    setInterval(() => spawnHearts(6), 2400);  
  </script>  
</body>  
</html>  
