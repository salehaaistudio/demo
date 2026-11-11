<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Solar Estimate in 60 Seconds | Heliora Solar</title>
<meta name="description" content="Enter your address. We scan your roof by satellite and send a custom solar estimate by email and text in about a minute.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,600;12..96,800&family=DM+Sans:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{--bg:#060E1C;--bg2:#0D1A33;--tx:#EAF2FF;--mute:#9DB0C8;--sun:#FFB020;--coral:#FF6B4A;--teal:#22D3A6;--blue:#3B82F6;--line:rgba(255,255,255,.12);
--head:'Bricolage Grotesque','Trebuchet MS',system-ui,sans-serif;--body:'DM Sans',system-ui,-apple-system,'Segoe UI',sans-serif}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth}
body{font-family:var(--body);background:var(--bg);color:var(--tx);line-height:1.6;overflow-x:hidden;-webkit-font-smoothing:antialiased}
h1,h2,h3{font-family:var(--head);line-height:1.08;letter-spacing:-.02em}
a{color:inherit}
:focus-visible{outline:3px solid var(--sun);outline-offset:3px}
.wrap{max-width:1180px;margin:0 auto;padding:0 24px;position:relative}

nav{position:fixed;inset:0 0 auto;z-index:20;padding:14px 0;transition:.3s}
nav.sc{background:rgba(6,14,28,.82);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
nav .wrap{display:flex;justify-content:space-between;align-items:center}
.logo{display:flex;align-items:center;gap:10px;font-family:var(--head);font-weight:800;font-size:1.3rem;text-decoration:none}
.logo i{width:26px;height:26px;border-radius:50%;background:radial-gradient(circle at 35% 35%,#FFE29A,var(--sun) 55%,var(--coral));animation:glow 3s ease-in-out infinite}
@keyframes glow{0%,100%{box-shadow:0 0 14px rgba(255,176,32,.6)}50%{box-shadow:0 0 34px rgba(255,176,32,1)}}
.nb{padding:9px 20px;border-radius:99px;background:linear-gradient(90deg,var(--sun),var(--coral));color:#1A1205;font-weight:700;text-decoration:none;font-size:.95rem}

.hero{position:relative;min-height:100vh;padding:130px 0 80px;overflow:hidden;display:flex;align-items:center}
.blob{position:absolute;border-radius:50%;filter:blur(90px);opacity:.55;animation:drift 14s ease-in-out infinite alternate}
.b1{width:520px;height:520px;background:var(--coral);top:-160px;right:-80px}
.b2{width:460px;height:460px;background:var(--blue);bottom:-180px;left:-120px;animation-delay:-5s}
.b3{width:340px;height:340px;background:var(--sun);top:30%;left:38%;opacity:.28;animation-delay:-9s}
@keyframes drift{to{transform:translate(60px,40px) scale(1.15)}}
.grid{position:absolute;inset:0;background-image:linear-gradient(var(--line) 1px,transparent 1px),linear-gradient(90deg,var(--line) 1px,transparent 1px);background-size:56px 56px;mask-image:radial-gradient(ellipse at 50% 40%,#000 20%,transparent 75%);opacity:.5}
.hero .wrap{display:grid;grid-template-columns:1.05fr .95fr;gap:52px;align-items:center}
.pill{display:inline-flex;align-items:center;gap:8px;padding:7px 16px;border:1px solid var(--line);border-radius:99px;background:rgba(255,255,255,.06);font-size:.9rem;margin-bottom:22px}
.pill b{width:8px;height:8px;border-radius:50%;background:var(--teal);animation:ping 1.6s infinite}
@keyframes ping{0%{box-shadow:0 0 0 0 rgba(34,211,166,.8)}100%{box-shadow:0 0 0 12px rgba(34,211,166,0)}}
.hero h1{font-size:clamp(2.4rem,5.6vw,4.4rem);font-weight:800}
.hero h1 span{background:linear-gradient(90deg,var(--sun),var(--coral),var(--sun));background-size:200% auto;-webkit-background-clip:text;background-clip:text;color:transparent;animation:flow 4s linear infinite}
@keyframes flow{to{background-position:200% center}}
.lead{margin:22px 0 28px;color:var(--mute);font-size:1.15rem;max-width:33em}
.scan{position:relative;max-width:480px}
.scan svg{width:100%;display:block}
.pn{fill:#1E3A66;stroke:#4F86D6;stroke-width:1;animation:pn 5.5s ease-in-out infinite}
@keyframes pn{0%,15%{fill:#1E3A66}30%,80%{fill:var(--sun)}95%,100%{fill:#1E3A66}}
.beam{animation:beam 5.5s ease-in-out infinite}
@keyframes beam{0%{transform:translateY(0);opacity:0}8%{opacity:1}40%{transform:translateY(150px);opacity:1}50%,100%{transform:translateY(150px);opacity:0}}
.tag{position:absolute;padding:9px 14px;border-radius:14px;background:rgba(13,26,51,.85);border:1px solid var(--line);backdrop-filter:blur(8px);font-size:.85rem;animation:float 4s ease-in-out infinite}
.tag strong{display:block;font-family:var(--head);font-size:1.2rem;color:var(--sun)}
.t1{top:2%;right:-4%}.t2{bottom:14%;left:-6%;animation-delay:-1.3s}.t3{bottom:-3%;right:6%;animation-delay:-2.4s}
@keyframes float{50%{transform:translateY(-12px)}}
.ex{font-size:.75rem;color:var(--mute);margin-top:10px}

.fw{position:relative;border-radius:26px;padding:2px;background:conic-gradient(from var(--a,0deg),var(--sun),var(--coral),var(--blue),var(--teal),var(--sun));animation:spin 6s linear infinite}
@property --a{syntax:'<angle>';initial-value:0deg;inherits:false}
@keyframes spin{to{--a:360deg}}
.card{border-radius:24px;background:linear-gradient(160deg,#0F1F3D,#0A1428);padding:32px}
.card h2{font-size:1.75rem}
.sub{color:var(--mute);margin:6px 0 18px;font-size:.98rem}
label{display:block;font-weight:700;font-size:.88rem;margin:14px 0 6px}
input[type=text],input[type=email],input[type=tel]{width:100%;font:inherit;color:var(--tx);padding:13px 14px;border:1.5px solid var(--line);border-radius:12px;background:rgba(255,255,255,.05);transition:.2s}
input::placeholder{color:#6F83A0}
input:focus{outline:none;border-color:var(--sun);box-shadow:0 0 0 4px rgba(255,176,32,.2);background:rgba(255,255,255,.08)}
input.bad{border-color:#FF5A4A;background:rgba(255,90,74,.1)}
.row{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.consent{display:flex;gap:10px;align-items:flex-start;margin:18px 0 6px;font-size:.8rem;color:var(--mute);font-weight:400}
.consent input{margin-top:3px;width:18px;height:18px;accent-color:var(--coral);flex:none}
.hp{position:absolute;left:-9999px}
.go{position:relative;overflow:hidden;width:100%;margin-top:14px;border:0;cursor:pointer;font:inherit;font-weight:700;font-size:1.08rem;color:#1A1205;padding:16px;border-radius:14px;background:linear-gradient(90deg,var(--sun),var(--coral));box-shadow:0 12px 30px rgba(255,107,74,.35);transition:transform .15s}
.go::after{content:"";position:absolute;top:0;left:-60%;width:40%;height:100%;background:linear-gradient(100deg,transparent,rgba(255,255,255,.55),transparent);transform:skewX(-20deg);animation:shine 3.2s infinite}
@keyframes shine{0%,60%{left:-60%}100%{left:140%}}
.go:hover{transform:translateY(-2px)}
.go:disabled{opacity:.6;cursor:wait}
.err{display:none;margin-top:12px;color:#FFB4A8;font-size:.92rem;background:rgba(255,90,74,.12);border-radius:10px;padding:10px 12px}
.fine{font-size:.78rem;color:var(--mute);margin-top:12px;text-align:center}
.state{display:none;text-align:center;padding:6px 0}
.state.on{display:block}
.timer{font-family:var(--head);font-weight:800;font-size:3.4rem;background:linear-gradient(90deg,var(--sun),var(--coral));-webkit-background-clip:text;background-clip:text;color:transparent}
.steps{list-style:none;padding:0;margin:16px auto 0;max-width:290px;text-align:left}
.steps li{padding:9px 0 9px 34px;position:relative;color:var(--mute);transition:.3s}
.steps li::before{content:"";position:absolute;left:4px;top:12px;width:16px;height:16px;border-radius:50%;border:2px solid var(--line)}
.steps li.act{color:var(--tx);font-weight:700}
.steps li.act::before{border-color:var(--sun);border-top-color:transparent;animation:rot .8s linear infinite}
.steps li.done{color:var(--tx)}
.steps li.done::before{background:var(--teal);border-color:var(--teal)}
@keyframes rot{to{transform:rotate(360deg)}}
.tick{width:76px;height:76px;border-radius:50%;background:var(--teal);margin:0 auto 14px;display:grid;place-items:center;animation:pop .5s cubic-bezier(.2,1.6,.4,1)}
@keyframes pop{from{transform:scale(0)}to{transform:scale(1)}}
.tick svg{width:38px;height:38px;stroke:#042;fill:none;stroke-width:5;stroke-linecap:round;stroke-linejoin:round}
.reset{margin-top:16px;background:none;border:0;color:var(--mute);text-decoration:underline;cursor:pointer;font:inherit}

.mq{border-block:1px solid var(--line);background:var(--bg2);overflow:hidden;padding:16px 0}
.mq div{display:flex;gap:48px;width:max-content;animation:mq 28s linear infinite;font-family:var(--head);font-weight:600;font-size:1.15rem;color:var(--mute)}
.mq span::before{content:"";display:inline-block;width:10px;height:10px;border-radius:50%;background:var(--sun);margin-right:14px}
@keyframes mq{to{transform:translateX(-50%)}}

.s{padding:96px 0;position:relative}
.s h2{font-size:clamp(1.9rem,3.8vw,2.9rem);max-width:17em}
.intro{color:var(--mute);margin-top:12px;max-width:40em;font-size:1.08rem}
.rv{opacity:0;transform:translateY(34px);transition:opacity .8s,transform .8s}
.rv.in{opacity:1;transform:none}
.flow{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-top:48px;position:relative}
.flow::before{content:"";position:absolute;top:34px;left:10%;right:10%;height:2px;background:linear-gradient(90deg,var(--sun),var(--coral),var(--blue));transform:scaleX(0);transform-origin:left;transition:transform 1.6s .3s}
.flow.in::before{transform:scaleX(1)}
.flow article{position:relative;padding:26px;border-radius:20px;background:rgba(255,255,255,.04);border:1px solid var(--line);transition:.3s}
.flow article:hover,.why div:hover{transform:translateY(-8px);border-color:var(--sun);box-shadow:0 20px 50px rgba(255,176,32,.15)}
.ic{width:56px;height:56px;border-radius:16px;display:grid;place-items:center;background:linear-gradient(135deg,var(--sun),var(--coral));margin-bottom:16px;position:relative;z-index:1}
.ic svg{width:28px;height:28px;stroke:#1A1205;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.flow h3{font-size:1.35rem;margin-bottom:8px}
.flow p,.why p{color:var(--mute)}
.prev{display:grid;grid-template-columns:1.05fr .95fr;gap:52px;align-items:center}
.mail{background:#fff;color:#10233B;border-radius:20px;overflow:hidden;box-shadow:0 30px 70px rgba(0,0,0,.5);transform:rotate(-2deg);transition:.4s}
.mail:hover{transform:rotate(0) scale(1.02)}
.mail .bar{background:#10233B;color:#C9D7E8;padding:12px 18px;font-size:.85rem}
.mail .bd{padding:22px}
.mail h3{font-size:1.3rem;margin-bottom:8px}
.kv{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin:16px 0}
.kv div{background:#EAF4FB;border-radius:12px;padding:12px 14px}
.kv small{display:block;color:#5B6B80;font-size:.8rem}
.kv strong{font-family:var(--head);font-size:1.4rem}
.mbtn{display:inline-block;background:var(--sun);font-weight:700;padding:11px 20px;border-radius:10px}
.note{font-size:.8rem;color:#5B6B80;margin-top:12px}
.calc{list-style:none;padding:0;margin-top:22px}
.calc li{padding:12px 0 12px 18px;border-left:4px solid var(--sun);margin-bottom:12px;color:var(--mute)}
.calc b{display:block;color:var(--tx)}
.why{display:grid;grid-template-columns:repeat(2,1fr);gap:22px;margin-top:44px}
.why div{padding:26px;border-radius:20px;background:rgba(255,255,255,.04);border:1px solid var(--line);transition:.3s}
.why h3{font-size:1.25rem;margin-bottom:6px}
details{border-bottom:1px solid var(--line);padding:18px 0;max-width:780px}
summary{cursor:pointer;font-weight:700;font-size:1.1rem;list-style:none;display:flex;justify-content:space-between;gap:16px}
summary::after{content:"+";color:var(--sun);font-size:1.6rem;line-height:1;transition:transform .25s}
details[open] summary::after{transform:rotate(45deg)}
details p{margin-top:10px;color:var(--mute);max-width:42em}
.cta{position:relative;text-align:center;padding:100px 24px;overflow:hidden;background:linear-gradient(180deg,var(--bg),#2A1530 60%,#6B2B2A)}
.cta .sun2{position:absolute;left:50%;bottom:-260px;width:520px;height:520px;margin-left:-260px;border-radius:50%;background:radial-gradient(circle,#FFE29A,var(--sun) 40%,transparent 70%);animation:pulse 4s ease-in-out infinite}
@keyframes pulse{50%{transform:scale(1.12);opacity:.8}}
.cta h2{position:relative;font-size:clamp(1.9rem,4vw,3rem);margin:0 auto 22px;max-width:14em}
.cta a{position:relative;display:inline-block;background:var(--tx);color:#10233B;padding:16px 34px;border-radius:14px;font-weight:700;text-decoration:none;transition:.2s}
.cta a:hover{transform:translateY(-3px) scale(1.04)}
footer{background:#040A15;color:#7F93AD;padding:28px 0;font-size:.88rem}
footer .wrap{display:flex;justify-content:space-between;flex-wrap:wrap;gap:10px}

@media(max-width:900px){
 .hero{padding:110px 0 60px;min-height:0}.hero .wrap,.prev{grid-template-columns:1fr}
 .scan{margin:10px auto 0;max-width:380px}.t1{right:0}.t2{left:0}
 .flow,.why{grid-template-columns:1fr}.flow::before{display:none}.s{padding:70px 0}
}
@media(max-width:480px){.row{grid-template-columns:1fr}.card{padding:24px 20px}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.rv{opacity:1;transform:none}}
</style>
</head>

<body>

<nav id="nav">
 <div class="wrap">
  <a class="logo" href="#top"><i></i>Heliora Solar</a>
  <a class="nb" href="#quote">Get my estimate</a>
 </div>
</nav>

<header class="hero" id="top">
 <div class="blob b1"></div>
 <div class="blob b2"></div>
 <div class="blob b3"></div>
 <div class="grid"></div>

 <div class="wrap">
  <div>
   <div class="pill"><b></b>Estimate delivered in about 60 seconds</div>
   <h1>Your roof, scanned from space. <span>Your solar estimate, in a minute.</span></h1>
   <p class="lead">Enter your address. We read your roof from satellite data and send a custom proposal to your inbox and phone. No waiting for a callback.</p>

   <div class="scan">
    <svg viewBox="0 0 400 290" role="img" aria-label="Animation of a roof being scanned from above while solar panels light up">
     <rect x="20" y="20" width="360" height="250" rx="18" fill="#0B1730" stroke="#2B4A7F"/>
     <rect x="60" y="50" width="280" height="190" rx="8" fill="#223B63"/>
     <line x1="200" y1="50" x2="200" y2="240" stroke="#0B1730" stroke-width="3"/>
     <g id="pg"></g>
     <g class="beam">
      <rect x="40" y="46" width="320" height="14" rx="6" fill="rgba(255,255,255,.35)"/>
      <rect x="40" y="52" width="320" height="2" fill="#fff"/>
     </g>
    </svg>
    <div class="tag t1">Panels<strong>24</strong></div>
    <div class="tag t2">System size<strong>9.6 kW</strong></div>
    <div class="tag t3">Est. savings<strong>$1,980 / yr</strong></div>
    <p class="ex">Illustration with example numbers.</p>
   </div>
  </div>

  <div class="fw" id="quote">
   <div class="card">
    <div id="formView">
     <h2>Get your solar estimate</h2>
     <p class="sub">Enter your full home address from any country.</p>

     <form id="f" novalidate>
      <label for="name">Full name</label>
      <input id="name" name="name" type="text" autocomplete="name" placeholder="Jordan Smith" required>

      <div class="row">
       <div>
        <label for="email">Email</label>
        <input id="email" name="email" type="email" autocomplete="email" placeholder="you@email.com" required>
       </div>
       <div>
        <label for="phone">Mobile number</label>
        <input id="phone" name="phone" type="tel" autocomplete="tel" placeholder="(555) 123-4567" required>
       </div>
      </div>

      <label for="address">Home address</label>
      <input id="address" name="address" type="text" autocomplete="street-address" placeholder="Street, city, postal code, country" required>

      <input class="hp" type="text" name="website" tabindex="-1" autocomplete="off" aria-hidden="true">

      <label class="consent">
       <input type="checkbox" id="consent">
       <span>I agree to receive my estimate by email and text message. Message and data rates may apply.</span>
      </label>

      <button class="go" id="btn" type="submit">Get my estimate</button>
      <div class="err" id="err" role="alert"></div>
      <p class="fine">Estimates use satellite data and are not a final quote.</p>
     </form>
    </div>

    <div class="state" id="loadView" aria-live="polite">
     <div class="timer" id="timer">0s</div>
     <p>Building your estimate...</p>
     <ul class="steps" id="steps">
      <li>Locating your home</li>
      <li>Scanning your roof</li>
      <li>Calculating your savings</li>
      <li>Writing your proposal</li>
      <li>Sending email and text</li>
     </ul>
    </div>

    <div class="state" id="doneView" aria-live="polite">
     <div class="tick">
      <svg viewBox="0 0 24 24"><path d="M5 12.5l4.5 4.5L19 7.5"/></svg>
     </div>
     <h2>Your estimate is on its way</h2>
     <p class="sub" id="doneMsg">Check your email and phone in the next minute.</p>
     <button class="reset" id="again" type="button">Request another estimate</button>
    </div>
   </div>
  </div>
 </div>
</header>

<div class="mq" aria-hidden="true">
 <div>
  <span>Satellite roof scan</span>
  <span>Estimate by email</span>
  <span>Estimate by text</span>
  <span>Savings in plain numbers</span>
  <span>Book a call in one click</span>
  <span>Satellite roof scan</span>
  <span>Estimate by email</span>
  <span>Estimate by text</span>
  <span>Savings in plain numbers</span>
  <span>Book a call in one click</span>
 </div>
</div>

<section class="s" id="how">
 <div class="wrap">
  <h2 class="rv">From address to proposal in three steps</h2>
  <p class="intro rv">The estimate reaches you while you are still thinking about it.</p>

  <div class="flow rv">
   <article>
    <div class="ic">
     <svg viewBox="0 0 24 24"><path d="M12 21s-7-6.2-7-11a7 7 0 0114 0c0 4.8-7 11-7 11z"/><circle cx="12" cy="10" r="2.5"/></svg>
    </div>
    <h3>Share your address</h3>
    <p>Tell us where you live and how to reach you.</p>
   </article>

   <article>
    <div class="ic">
     <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="4"/><path d="M12 2v3M12 19v3M2 12h3M19 12h3M4.9 4.9l2.1 2.1M17 17l2.1 2.1M19.1 4.9L17 7M7 17l-2.1-2.1"/></svg>
    </div>
    <h3>We scan your roof</h3>
    <p>Satellite data shows how many panels fit and how much sun they get.</p>
   </article>

   <article>
    <div class="ic">
     <svg viewBox="0 0 24 24"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="M3 7l9 6 9-6"/></svg>
    </div>
    <h3>Get your estimate</h3>
    <p>A personal proposal arrives by email and text, with your next step.</p>
   </article>
  </div>
 </div>
</section>

<section class="s" style="background:var(--bg2)">
 <div class="wrap prev">
  <div class="mail rv" role="img" aria-label="Sample estimate email">
   <div class="bar">Subject: Your solar estimate for 123 Maple Street</div>
   <div class="bd">
    <h3>Hi Jordan, here is your estimate</h3>
    <p>We scanned your roof. This is what a system could look like for your home.</p>
    <div class="kv">
     <div><small>Solar panels</small><strong>24</strong></div>
     <div><small>System size</small><strong>9.6 kW</strong></div>
     <div><small>Energy per year</small><strong>12,400 kWh</strong></div>
     <div><small>Yearly savings</small><strong>$1,980</strong></div>
    </div>
    <span class="mbtn">Book a time to talk</span>
    <p class="note">Sample only. Your numbers come from your own roof.</p>
   </div>
  </div>

  <div class="rv">
   <h2>Here is what lands in your inbox</h2>
   <p class="intro">A short, personal proposal with the numbers that matter, plus a link to pick a time with our team.</p>
   <ul class="calc">
    <li><b>System size</b>Panels that fit on your roof, times the power of each panel.</li>
    <li><b>Yearly energy</b>Based on how much sun your roof receives across the year.</li>
    <li><b>Savings and cost</b>Energy produced at your electricity rate, against the system price.</li>
   </ul>
  </div>
 </div>
</section>

<section class="s">
 <div class="wrap">
  <h2 class="rv">Why homeowners start with an estimate</h2>
  <div class="why rv">
   <div><h3>Based on your actual roof</h3><p>Not a national average. The numbers come from your home's own roof data.</p></div>
   <div><h3>Fast by design</h3><p>You hear back in about a minute, not days.</p></div>
   <div><h3>Clear numbers</h3><p>System size, yearly energy, estimated savings and cost in plain language.</p></div>
   <div><h3>Book when you are ready</h3><p>Pick a time to talk with our team, or keep the estimate and decide later.</p></div>
  </div>
 </div>
</section>

<section class="s" style="background:var(--bg2)">
 <div class="wrap">
  <h2 class="rv">Common questions</h2>
  <div class="rv" style="margin-top:30px">
   <details><summary>How accurate is the estimate?</summary><p>It uses satellite roof data and standard assumptions, so treat it as a close first look. Our team confirms details before any final quote.</p></details>
   <details><summary>What if you cannot find my home?</summary><p>Some addresses are missing from satellite data. If that happens we tell you, and a team member reviews your roof by hand.</p></details>
   <details><summary>Will someone call me right away?</summary><p>No. You get your estimate first and choose when to talk.</p></details>
   <details><summary>Does it cost anything?</summary><p>No. The estimate is free and carries no obligation.</p></details>
  </div>
 </div>
</section>

<div class="cta">
 <div class="sun2"></div>
 <h2 class="rv">Your roof is already getting the sun.</h2>
 <a href="#quote">Get my estimate</a>
</div>

<footer>
 <div class="wrap">
  <span>&copy; 2026 Heliora Solar.</span>
  <span>Contact: <a href="mailto:aminruhul7202@gmail.com">aminruhul7202@gmail.com</a></span>
  <span>Estimates are not final quotes.</span>
 </div>
</footer>

<script>
/* ====== PRODUCTION WEBHOOK SETTINGS ====== */
const WEBHOOK_URL = "https://n8n.hablu-programmer.com/webhook/heliora-solar-lead";
/* ========================================= */

(function(){
  let h = '';

  for(let r = 0; r < 4; r++){
    for(let c = 0; c < 6; c++){
      const x = 70 + c * 45 + (c >= 3 ? 8 : 0);
      const y = 60 + r * 43;

      h += '<rect class="pn" x="' + x + '" y="' + y +
        '" width="40" height="36" rx="3" style="animation-delay:' +
        (r * 0.55 + c * 0.07).toFixed(2) + 's"/>';
    }
  }

  document.getElementById('pg').innerHTML = h;
})();

(function(){
  const nav = document.getElementById('nav');

  addEventListener('scroll', () => {
    nav.classList.toggle('sc', scrollY > 30);
  }, {passive:true});

  const els = document.querySelectorAll('.rv');

  if(!('IntersectionObserver' in window)){
    els.forEach(e => e.classList.add('in'));
    return;
  }

  const io = new IntersectionObserver(es => {
    es.forEach(e => {
      if(e.isIntersecting){
        e.target.classList.add('in');
        io.unobserve(e.target);
      }
    });
  }, {threshold:.15});

  els.forEach(e => io.observe(e));
})();

const $ = id => document.getElementById(id);

const views = {
  form: $('formView'),
  load: $('loadView'),
  done: $('doneView')
};

function show(v){
  Object.entries(views).forEach(([k,el]) => {
    if(k === 'form'){
      el.style.display = (v === 'form') ? 'block' : 'none';
    } else {
      el.classList.toggle('on', k === v);
    }
  });
}

show('form');

let tmr, stp, t0;

function startProgress(){
  t0 = Date.now();

  const items = [...$('steps').children];
  let i = 0;

  items.forEach(li => li.className = '');
  items[0].className = 'act';

  $('timer').textContent = '0s';

  tmr = setInterval(() => {
    $('timer').textContent =
      Math.floor((Date.now() - t0) / 1000) + 's';
  }, 250);

  stp = setInterval(() => {
    if(i < items.length - 1){
      items[i].className = 'done';
      i++;
      items[i].className = 'act';
    }
  }, 2800);
}

function stopProgress(){
  clearInterval(tmr);
  clearInterval(stp);
}

function showErr(m){
  const e = $('err');
  e.textContent = m;
  e.style.display = 'block';
}

function clearErr(){
  $('err').style.display = 'none';

  document.querySelectorAll('#f .bad').forEach(x => {
    x.classList.remove('bad');
  });
}

/* ====== FORM SUBMISSION ====== */

$('f').addEventListener('submit', async (ev) => {

  ev.preventDefault();
  clearErr();

  const form = ev.currentTarget;

  // FIX: Safely get form fields by name.
  const field = (name) => form.elements.namedItem(name);

  const nameField = field('name');
  const emailField = field('email');
  const phoneField = field('phone');
  const addressField = field('address');
  const websiteField = field('website');

  if(!nameField || !emailField || !phoneField || !addressField || !websiteField){
    showErr('Form fields could not be found. Please refresh the page and try again.');
    return;
  }

  const d = {
    name: nameField.value.trim(),
    email: emailField.value.trim(),
    phone: phoneField.value.trim(),
    address: addressField.value.trim(),
    consent: $('consent').checked
  };

  // Honeypot spam protection.
  if(websiteField.value.trim()){
    return;
  }

  const bad = [];

  if(d.name.length < 2){
    bad.push('name');
  }

  if(!/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test(d.email)){
    bad.push('email');
  }

  const digits = d.phone.replace(/\D/g, '');
  const hasCountryCode = d.phone.trim().startsWith('+');

  const validPhone = hasCountryCode
    ? (digits.length >= 8 && digits.length <= 15)
    : (digits.length === 10 || (digits.length === 11 && digits[0] === '1'));

  if(!validPhone){
    bad.push('phone');
  }

  if(d.address.length < 8){
    bad.push('address');
  }

  if(bad.length){
    bad.forEach(name => {
      field(name).classList.add('bad');
    });

    showErr('Please check the highlighted fields. Enter a valid phone number with country code (for example +1...) and your complete home address, including country.');
    return;
  }

  if(!d.consent){
    showErr('Please tick the box to receive your estimate by email and text.');
    return;
  }

  // Normalize phone number.
  d.phone = hasCountryCode
    ? ('+' + digits)
    : (digits.length === 11 ? '+' + digits : '+1' + digits);

  const button = $('btn');

  button.disabled = true;
  show('load');
  startProgress();

  try{

    const response = await fetch(WEBHOOK_URL, {
      method: 'POST',
      headers: {
        'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8'
      },
      body: new URLSearchParams(d)
    });

    if(!response.ok){

      const responseText = await response.text().catch(() => '');

      throw new Error(
        'Webhook returned HTTP ' + response.status +
        (responseText ? ' — ' + responseText.slice(0,180) : '')
      );
    }

    stopProgress();

    const seconds = Math.max(
      1,
      Math.round((Date.now() - t0) / 1000)
    );

    $('doneMsg').textContent =
      'Request received in ' + seconds +
      's. Check your email and phone in the next minute.';

    show('done');

  }catch(error){

    stopProgress();
    show('form');

    button.disabled = false;

    const detail = String(
      error && error.message ? error.message : error
    );

    showErr(
      detail.includes('Failed to fetch')
        ? 'The request could not be completed. Check that the n8n workflow is Active, the Production Webhook path is correct, and the webhook response allows this website origin (CORS).'
        : 'Request failed: ' + detail
    );

    console.error('Heliora Solar webhook error:', error);
  }

});

/* ====== RESET FORM ====== */

$('again').addEventListener('click', () => {
  $('f').reset();
  $('btn').disabled = false;
  clearErr();
  show('form');
});

</script>

</body>
</html>
