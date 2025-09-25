# For-bea<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>For Bea</title>
<style>
  :root{
    --bg:#0f1724;
    --card:#0b1220;
    --accent:#f6c1d9;
    --muted:#9aa6b2;
    --glass: rgba(255,255,255,0.04);
    --radius:16px;
  }
  *{box-sizing:border-box}
  html,body{height:100%;margin:0;font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;}
  body{
    background:
      radial-gradient(600px 400px at 10% 10%, rgba(246,193,217,0.06), transparent 10%),
      radial-gradient(500px 350px at 90% 90%, rgba(120,180,255,0.03), transparent 10%),
      var(--bg);
    color:#e6eef6;
    display:flex;
    align-items:center;
    justify-content:center;
    padding:32px;
  }

  .container{
    width:min(900px,96vw);
    background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border-radius:var(--radius);
    box-shadow: 0 10px 30px rgba(2,6,23,0.6), inset 0 1px 0 rgba(255,255,255,0.02);
    overflow:hidden;
    display:flex;
    gap:0;
  }

  .left{
    flex:1 1 380px;
    padding:36px;
    background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(0,0,0,0.02));
    display:flex;
    flex-direction:column;
    justify-content:center;
  }
  .title{
    font-size:28px;
    margin:0 0 8px 0;
    letter-spacing:0.2px;
  }
  .subtitle{
    color:var(--muted);
    margin:0 0 20px 0;
    font-size:14px;
  }

  .envelope{
    margin-top:12px;
    width:120px;
    height:80px;
    position:relative;
    cursor:pointer;
  }
  .envelope .flap{
    position:absolute;
    left:0;right:0;top:0;height:50%;
    background:linear-gradient(180deg,#1b2a40,#11202f);
    transform-origin:top center;
    border-radius:8px 8px 0 0;
    transition: transform 650ms cubic-bezier(.2,.9,.3,1);
  }
  .envelope .body{
    position:absolute;left:0;right:0;bottom:0;height:60%;
    background:linear-gradient(180deg,#0f1b2a,#071018);
    border-radius:0 0 8px 8px;
    display:flex;align-items:center;justify-content:center;color:var(--muted);
    font-size:13px;
    padding:10px;
  }

  .right{
    flex:1 1 420px;
    padding:36px;
    border-left:1px solid rgba(255,255,255,0.02);
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(0,0,0,0.02));
  }

  .letter{
    background:var(--card);
    padding:28px;
    border-radius:12px;
    min-height:220px;
    box-shadow: 0 8px 20px rgba(2,6,23,0.55);
    transform-origin: top center;
    opacity:0;
    transform: translateY(18px) scale(.995);
    transition: opacity 600ms ease, transform 600ms cubic-bezier(.2,.9,.3,1);
    white-space:pre-wrap;
  }

  .letter.visible{
    opacity:1;
    transform: translateY(0) scale(1);
  }

  .letter h2{margin:0 0 12px 0;font-size:20px;color:var(--accent)}
  .letter p{margin:0 0 12px 0;color:#dfe9f3;line-height:1.6}
  .small{font-size:13px;color:var(--muted);margin-top:8px}

  .actions{margin-top:18px;display:flex;gap:12px}
  .btn{
    padding:10px 14px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.06);
    color:var(--accent);cursor:pointer;font-weight:600;font-size:14px;
  }
  .btn.ghost{background:transparent;color:var(--muted);border:1px dashed rgba(255,255,255,0.03)}
  .copy-note{font-size:13px;color:var(--muted);margin-top:10px}

  /* small screens */
  @media (max-width:760px){
    .container{flex-direction:column}
    .left,.right{padding:20px}
    .envelope{margin:14px 0}
  }
</style>
</head>
<body>
<div class="container" role="main" aria-labelledby="main-title">
  <div class="left">
    <h1 class="title" id="main-title">For Bea</h1>
    <p class="subtitle">Open the envelope when you're ready. No rush — just press it gently.</p>

    <div class="envelope" id="envelope" title="Open letter">
      <div class="flap" id="flap"></div>
      <div class="body">A message for you</div>
    </div>

    <div class="small">Hint: you can click the envelope or the "Open letter" button on the right.</div>
  </div>

  <div class="right">
    <div class="letter" id="letter">
      <h2>Dear Bea,</h2>
      <p id="letter-text">
Hi Bea,

I just want to be honest about something I’ve been keeping since last school year. I like you, Bea! Gikan pa sa duty nato. I don’t know where or when it started, but I just realized it from the moment na nailang nako every time you showed up. I love listening to you when you share your stories and even your random thoughts. I like how you care for others, even in a silent way. I love how you cherish the people that surround you and support you.

To be honest, when you asked kun I like girls, I also questioned myself if I do like girls or if it was just because of influence from my friends. But when I see you and talk to you, ahhh ikaw diay you’re the only exception. I know you like men, this is the reason why I distanced myself, because I didn’t want to make things awkward between you and me. I also like men, but when I see you, you’re different. 
I feel different.

I always listen to “The Only Exception” by Paramore and it always reminds me of you, Bee. I like you, Bee. I don’t want to put pressure on you or make you feel any urgency to respond to my message. That’s not what I want, because this message is just to tell you that I like you. I’m sorry if I ever did something that made you feel uncomfortable. I hope this message will stay just between us, because I will keep this at the bottom of my heart. This is my first-ever confession. I hope you understand if makulbaan ko when I see you after this message hehe. Anyway see you around, Bee!
      </p>

      <p class="small">— From someone who thinks you're wonderful</p>
    </div>

    <div class="actions">
      <button class="btn" id="openBtn">Open letter</button>
      <button class="btn ghost" id="revealPassBtn">Make private (password)</button>
    </div>

    <div class="copy-note" id="copyNote">When you're ready to send: copy the URL from your browser and paste it into your message.</div>
  </div>
</div>

<script>
  const flap = document.getElementById('flap');
  const envelope = document.getElementById('envelope');
  const openBtn = document.getElementById('openBtn');
  const letter = document.getElementById('letter');
  const revealPassBtn = document.getElementById('revealPassBtn');

  let opened = false;
  function openLetter() {
    if (opened) return;
    opened = true;
    flap.style.transform = 'rotateX(180deg) translateY(-6px)';
    setTimeout(()=> letter.classList.add('visible'), 520);
  }

  envelope.addEventListener('click', openLetter);
  openBtn.addEventListener('click', openLetter);

  // Simple client-side "password protect" (not secure, but hides letter unless password entered)
  revealPassBtn.addEventListener('click', ()=>{
    const pass = prompt('Set a short password for this letter (share it separately with Bea):','');
    if (!pass) return alert('No password set.');
    // store a hashed version in memory (very small obfuscation)
    const key = btoa(pass);
    localStorage.setItem('letter_key', key);
    // hide letter by default and require pass to view
    letter.classList.remove('visible');
    flap.style.transform = 'none';
    opened = false;
    const check = () => {
      const attempt = prompt('Enter the password to open the letter:','');
      if (!attempt) return;
      if (btoa(attempt) === localStorage.getItem('letter_key')){
        openLetter();
      } else {
        alert('Wrong password.');
      }
    };
    if (confirm('Now test entering the password?')) check();
    // change the reveal button to now be "Enter password"
    revealPassBtn.textContent = 'Enter password';
    revealPassBtn.onclick = check;
  });

  // Small accessibility: allow Enter key to open when envelope focused
  envelope.tabIndex = 0;
  envelope.addEventListener('keydown', (e)=>{ if(e.key === 'Enter') openLetter(); });
</script>
</body>
</html>
