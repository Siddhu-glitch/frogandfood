
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>For Likhitha 🌸</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
/* --- THEMES & CSS VARIABLES --- */
:root {
  --bg-top: #ffd9eb;
  --bg-mid: #eadfff;
  --bg-bottom: #dff4ff;
  --glass-bg: rgba(255, 255, 255, 0.35);
  --card-bg: rgba(255, 255, 255, 0.45);
  --text-dark: #555;
  --text-light: #666;
  --btn-grad-1: #ffb8d3;
  --btn-grad-2: #c9b9ff;
  --celestial-color: #fff;
  --celestial-glow: rgba(255, 255, 255, 0.8);
}

/* SUNSET THEME */
body.theme-sunset {
  --bg-top: #ffb7b2;
  --bg-mid: #ffdac1;
  --bg-bottom: #e2f0cb;
  --glass-bg: rgba(255, 255, 255, 0.25);
  --btn-grad-1: #ffb7b2;
  --btn-grad-2: #ffdac1;
  --celestial-color: #ffdfba;
}

/* NIGHT THEME */
body.theme-night {
  --bg-top: #1a1a2e;
  --bg-mid: #16213e;
  --bg-bottom: #0f3460;
  --glass-bg: rgba(15, 20, 30, 0.5);
  --card-bg: rgba(255, 255, 255, 0.1);
  --text-dark: #e0e0e0;
  --text-light: #b0b0b0;
  --btn-grad-1: #4a4e69;
  --btn-grad-2: #22223b;
  --celestial-color: #fca311;
}

/* HEADACHE MODE (Dims everything gently) */
body.headache-mode {
  filter: brightness(0.55) contrast(0.9) saturate(0.8);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
  -webkit-tap-highlight-color: transparent;
  transition: background 1.5s ease, filter 1.5s ease;
}

body {
  overflow: hidden;
  height: 100vh;
  background: linear-gradient(180deg, var(--bg-top), var(--bg-mid), var(--bg-bottom));
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--text-dark);
}

/* AMBIENT BACKGROUND ELEMENTS */
.cloud { position: absolute; font-size: 60px; opacity: 0.6; animation: drift 40s linear infinite; z-index: 0; }
.cloud1 { top: 15%; left: -10%; }
.cloud2 { top: 40%; left: -20%; animation-delay: 15s; font-size: 80px; }

@keyframes drift {
  0% { transform: translateX(-10vw); }
  100% { transform: translateX(110vw); }
}

.firefly {
  position: absolute; width: 4px; height: 4px; background: #e2f0cb; border-radius: 50%;
  box-shadow: 0 0 10px 2px #e2f0cb; animation: flicker 3s infinite alternate, wander 10s infinite ease-in-out;
  opacity: 0; z-index: 1;
}

@keyframes flicker { 0% { opacity: 0; } 50% { opacity: 0.8; } 100% { opacity: 0; } }
@keyframes wander { 0% { transform: translate(0, 0); } 50% { transform: translate(30px, -30px); } 100% { transform: translate(-20px, 20px); } }

.shooting-star {
  position: absolute; width: 100px; height: 2px; background: linear-gradient(90deg, white, transparent);
  top: 10%; right: -10%; transform: rotate(-45deg); animation: shoot 8s infinite linear; opacity: 0;
}
@keyframes shoot { 0% { right: -10%; top: 10%; opacity: 1; } 20% { right: 110%; top: 100%; opacity: 0; } 100% { opacity: 0; } }

/* POND & FLOATING ICONS */
.floating-icon {
  position: absolute; font-size: 45px; z-index: 2; cursor: pointer; transition: transform 0.3s ease;
}
.floating-icon:hover { transform: scale(1.1); filter: drop-shadow(0 0 8px rgba(255,255,255,0.6)); }

/* ADDED SUNFLOWERS & PINK LOTUS TO POND */
.lotus-pond { 
  bottom: 5%; width: 100%; text-align: center; position: absolute; z-index: 1; 
  font-size: 45px; letter-spacing: 15px; animation: gentleSway 6s infinite alternate; 
}

.petal { position: absolute; font-size: 22px; animation: fall 15s infinite linear; opacity: 0.7; z-index: 1; }
@keyframes fall { 0% { transform: translateY(-10vh) rotate(0deg); opacity: 0.7; } 100% { transform: translateY(110vh) rotate(360deg); opacity: 0; } }
@keyframes gentleSway { 0% { transform: translateX(-10px); } 100% { transform: translateX(10px); } }

.heart1 { top: 20%; right: 15%; animation: floatGentle 5s infinite ease-in-out; }

/* THE FROGS */
.frog-wrapper { position: absolute; animation: floatGentle 6s infinite ease-in-out; cursor: pointer; z-index: 5; }
.frog-wrapper .lilypad { position: absolute; bottom: -15px; left: -5px; font-size: 55px; z-index: -1; }
.frog-wrapper .frog { font-size: 50px; }

.fw1 { top: 22%; left: 8%; }
.fw2 { bottom: 18%; right: 10%; animation-delay: 2s; }

@keyframes floatGentle { 0% { transform: translateY(0px); } 50% { transform: translateY(-15px); } 100% { transform: translateY(0px); } }

/* BOOP ANIMATION */
.boop { animation: popSpin 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275) !important; }
@keyframes popSpin { 0% { transform: scale(1); } 50% { transform: scale(1.3) rotate(15deg); } 100% { transform: scale(1); } }

/* MAIN CONTAINER */
.container {
  width: 92%; max-width: 430px; height: 92vh; overflow-y: auto; background: var(--glass-bg);
  backdrop-filter: blur(25px); border-radius: 32px; border: 1px solid rgba(255, 255, 255, 0.3);
  padding: 25px 20px 30px; position: relative; z-index: 10; box-shadow: 0 15px 40px rgba(0,0,0,0.1);
  display: flex; flex-direction: column; align-items: center;
}
.container::-webkit-scrollbar { width: 0; }

/* CELESTIAL BODY (Sun/Moon) */
.celestial {
  width: 90px; height: 90px; border-radius: 50%; background: var(--celestial-color); margin: 0 auto;
  display: flex; justify-content: center; align-items: center; font-size: 40px; transition: 1.5s;
  box-shadow: 0 0 30px var(--celestial-glow); animation: pulse 4s infinite alternate;
}
@keyframes pulse { to { transform: scale(1.05); box-shadow: 0 0 45px var(--celestial-glow); } }

/* TYPEWRITER MESSAGE BOX */
.message-box {
  background: var(--card-bg); width: 100%; border-radius: 20px; padding: 15px; margin-top: 15px;
  min-height: 80px; display: flex; align-items: center; justify-content: center; text-align: center;
  font-size: 14px; font-weight: 500; color: var(--text-dark); border: 1px dashed rgba(255,255,255,0.5);
  line-height: 1.6;
}

/* CONTROLS */
.controls { display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; margin-top: 20px; width: 100%; }
.btn {
  border: none; padding: 10px 15px; border-radius: 20px; background: linear-gradient(145deg, var(--btn-grad-1), var(--btn-grad-2));
  color: white; font-size: 13px; cursor: pointer; transition: 0.3s; box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}
.btn:hover { transform: scale(1.05); }

/* BREATHING ORB */
.orb {
  width: 100px; height: 100px; border-radius: 50%; background: radial-gradient(circle, var(--btn-grad-1), var(--btn-grad-2));
  margin: 30px auto 10px; display: flex; justify-content: center; align-items: center; color: white;
  animation: breatheOrb 8s infinite ease-in-out; opacity: 0.9; box-shadow: 0 0 20px var(--btn-grad-1);
}
@keyframes breatheOrb { 0% { transform: scale(1); opacity: 0.7; } 50% { transform: scale(1.4); opacity: 1; } 100% { transform: scale(1); opacity: 0.7; } }
.breath-text { text-align: center; font-size: 14px; color: var(--text-light); }

/* MAGIC FLOAT ANIMATION FOR TAPPED EMOJIS */
.magic-float {
  position: absolute;
  font-size: 35px;
  z-index: 100;
  pointer-events: none;
  transition: all 1.5s cubic-bezier(0.25, 1, 0.5, 1);
  opacity: 1;
}

</style>
</head>
<body>

<div class="cloud cloud1">☁️</div>
<div class="cloud cloud2">☁️</div>
<div class="shooting-star"></div>

<div class="lotus-pond">🪷 🌻 🪷 🌻 🪷</div>

<div class="floating-icon heart1">🧡</div>

<div class="frog-wrapper fw1" onclick="tapFrog(this)">
  <div class="lilypad">🍃</div>
  <div class="frog">🐸</div>
</div>
<div class="frog-wrapper fw2" onclick="tapFrog(this)">
  <div class="lilypad">🍃</div>
  <div class="frog">🐸</div>
</div>

<audio id="rainAudio" loop><source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_c8c8e56d1f.mp3" type="audio/mp3"></audio>
<audio id="lofiAudio" loop><source src="https://cdn.pixabay.com/download/audio/2022/05/27/audio_1808fbf07a.mp3" type="audio/mp3"></audio>
<audio id="popSound"><source src="https://actions.google.com/sounds/v1/animals/frog_croak.ogg" type="audio/ogg"></audio>

<div class="container">
  <div class="celestial" id="celestial">☀️</div>
  
  <h1 style="text-align:center; margin-top:15px; font-size:26px;">For Likhitha 🌸</h1>
  
  <div class="message-box" id="messageBox">
    Tap a frog to say hello... 🐸
  </div>

  <div class="orb">Breathe</div>
  <div class="breath-text" id="breathText">Inhale slowly...</div>

  <div class="controls">
    <button class="btn" onclick="toggleHeadacheMode()">🕶️ Headache Mode</button>
    <button class="btn" onclick="cycleTheme()">🌗 Change Sky</button>
    <button class="btn" onclick="toggleAudio('rain')">🌧️ Rain</button>
    <button class="btn" onclick="toggleAudio('lofi')">📻 Lo-Fi</button>
  </div>
  
  <p style="text-align:center; font-size:12px; color:var(--text-light); margin-top:25px; font-style:italic;">
    “A tiny peaceful corner made with care 🧡”
  </p>
</div>

<script>
// --- BREATHING LOGIC ---
const breathText = document.getElementById("breathText");
let inhale = true;
setInterval(() => {
  breathText.innerText = inhale ? "Exhale gently..." : "Inhale slowly...";
  inhale = !inhale;
}, 4000);

// --- FROG TYPEWRITER QUOTES ---
const quotes = [
  "Frog says: It's okay to do absolutely nothing right now. 🌿",
  "Sending a pink lotus and a sunflower just for you! 🪷🌻",
  "Close your eyes. Let the rain wash the headache away. 🌧️",
  "You are safe here in this little pond. 🐸",
  "Frog promises: The pressure in your head will soften soon. 🧡",
  "Breathe in the cool air, breathe out the tension. 🌬️",
  "Even the darkest night has bright fireflies. ✨"
];
let isTyping = false;

function tapFrog(element) {
  // 1. Boop animation
  element.classList.remove('boop');
  void element.offsetWidth; // trigger reflow
  element.classList.add('boop');
  
  // 2. Play REAL frog croak sound
  let pop = document.getElementById('popSound');
  pop.volume = 0.5; // Slightly louder so the croak comes through clear
  pop.currentTime = 0;
  pop.play().catch(()=>{}); 

  // 3. ✨ MAGIC FEATURE: Spawn Pink Lotus & Sunflower ✨
  const rect = element.getBoundingClientRect();
  const magicEmojis = ['🪷', '🌻'];
  
  magicEmojis.forEach((emoji, index) => {
    let el = document.createElement('div');
    el.innerText = emoji;
    el.className = 'magic-float';
    // Position them exactly where the frog was clicked
    el.style.left = (rect.left + 15) + 'px';
    el.style.top = (rect.top - 10) + 'px';
    document.body.appendChild(el);

    // Animate them floating up and out
    setTimeout(() => {
      // Lotus goes left, Sunflower goes right
      const xMove = index === 0 ? -40 : 40; 
      el.style.transform = `translate(${xMove}px, -120px) scale(1.3) rotate(${xMove/2}deg)`;
      el.style.opacity = '0';
    }, 50);

    // Remove from code after animation finishes
    setTimeout(() => {
      el.remove();
    }, 1500);
  });

  // 4. Typewriter effect
  if(isTyping) return;
  isTyping = true;
  const msgBox = document.getElementById('messageBox');
  msgBox.innerText = "";
  const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
  
  let i = 0;
  const typing = setInterval(() => {
    msgBox.innerText += randomQuote.charAt(i);
    i++;
    if(i >= randomQuote.length) {
      clearInterval(typing);
      isTyping = false;
    }
  }, 45); // typing speed
}

// --- AUDIO LOGIC ---
const rain = document.getElementById('rainAudio');
const lofi = document.getElementById('lofiAudio');
rain.volume = 0.3; lofi.volume = 0.2;
let currentTrack = null;

function toggleAudio(type) {
  const track = type === 'rain' ? rain : lofi;
  const otherTrack = type === 'rain' ? lofi : rain;
  
  otherTrack.pause();
  if (currentTrack === track && !track.paused) {
    track.pause();
    currentTrack = null;
  } else {
    track.play();
    currentTrack = track;
  }
}

// --- THEME CYCLING (Day -> Sunset -> Night) ---
const themes = ['theme-day', 'theme-sunset', 'theme-night'];
const celestialIcons = ['☀️', '🌅', '🌙'];
let themeIndex = 0;

function cycleTheme() {
  document.body.classList.remove(themes[themeIndex]);
  themeIndex = (themeIndex + 1) % themes.length;
  if(themes[themeIndex] !== 'theme-day') {
    document.body.classList.add(themes[themeIndex]);
  }
  document.getElementById('celestial').innerText = celestialIcons[themeIndex];
}

// --- HEADACHE MODE ---
function toggleHeadacheMode() {
  document.body.classList.toggle('headache-mode');
}

// --- GENERATE FIREFLIES & PETALS ---
for(let i=0; i<15; i++) {
  let firefly = document.createElement('div');
  firefly.className = 'firefly';
  firefly.style.left = Math.random() * 100 + 'vw';
  firefly.style.top = Math.random() * 100 + 'vh';
  firefly.style.animationDelay = Math.random() * 5 + 's';
  document.body.appendChild(firefly);
}

// Added Sunflowers to the falling petals mix
const petalEmojis = ['🌸', '🍃', '✨', '🌻', '🪷'];
setInterval(() => {
  let petal = document.createElement('div');
  petal.className = 'petal';
  petal.innerText = petalEmojis[Math.floor(Math.random() * petalEmojis.length)];
  petal.style.left = Math.random() * 100 + 'vw';
  document.body.appendChild(petal);
  setTimeout(() => petal.remove(), 15000);
}, 2500);
</script>
</body>
</html>
