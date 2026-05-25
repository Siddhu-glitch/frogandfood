<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Likhitha 🌸</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Poppins',sans-serif;
}

body{
  overflow:hidden;
  height:100vh;
  background:linear-gradient(180deg,#ffd9eb,#eadfff,#dff4ff);
  position:relative;
  display:flex;
  justify-content:center;
  align-items:center;
  color:#555;
}

/* BACKGROUND BLURS */

.blur{
  position:absolute;
  width:350px;
  height:350px;
  border-radius:50%;
  filter:blur(100px);
  opacity:0.5;
  animation:float 8s infinite alternate ease-in-out;
}

.blur1{
  background:#ff9ecb;
  top:-100px;
  left:-100px;
}

.blur2{
  background:#a7cfff;
  bottom:-100px;
  right:-100px;
}

@keyframes float{
  from{
    transform:translateY(0px);
  }

  to{
    transform:translateY(30px);
  }
}

/* STARS */

.star{
  position:absolute;
  width:4px;
  height:4px;
  border-radius:50%;
  background:white;
  opacity:0.8;
  animation:twinkle 3s infinite alternate;
}

@keyframes twinkle{
  from{
    opacity:0.3;
  }

  to{
    opacity:1;
  }
}

/* LOTUS */

.lotus{
  position:absolute;
  font-size:52px;
  animation:lotusFloat 7s infinite alternate ease-in-out;
  z-index:1;
}

.lotus1{
  top:8%;
  right:8%;
}

.lotus2{
  bottom:10%;
  left:8%;
  animation-delay:2s;
}

@keyframes lotusFloat{
  from{
    transform:translateY(0px) rotate(-5deg);
  }

  to{
    transform:translateY(20px) rotate(5deg);
  }
}

/* SUNFLOWERS */

.sunflower{
  position:absolute;
  font-size:48px;
  z-index:1;
  animation:sunflowerMove 9s infinite alternate ease-in-out;
}

.sunflower1{
  top:16%;
  left:38%;
}

.sunflower2{
  bottom:16%;
  right:32%;
  animation-delay:2s;
}

@keyframes sunflowerMove{
  from{
    transform:rotate(-4deg) translateY(0px);
  }

  to{
    transform:rotate(6deg) translateY(-12px);
  }
}

/* HEARTS */

.heart{
  position:absolute;
  font-size:28px;
  animation:heartFloat 5s infinite ease-in-out;
}

.heart1{
  top:28%;
  right:20%;
}

.heart2{
  bottom:25%;
  left:20%;
  animation-delay:2s;
}

.heart3{
  top:55%;
  right:10%;
  animation-delay:4s;
}

@keyframes heartFloat{
  0%{
    transform:translateY(0px);
  }

  50%{
    transform:translateY(-15px);
  }

  100%{
    transform:translateY(0px);
  }
}

/* FROGS */

.frog{
  position:absolute;
  font-size:48px;
  z-index:1;
  animation:frogBounce 5s infinite ease-in-out;
}

.frog1{
  top:20%;
  left:6%;
}

.frog2{
  bottom:18%;
  right:8%;
  animation-delay:2s;
}

.frog3{
  top:70%;
  left:45%;
  animation-delay:4s;
}

@keyframes frogBounce{
  0%{
    transform:translateY(0px);
  }

  50%{
    transform:translateY(-18px);
  }

  100%{
    transform:translateY(0px);
  }
}

/* MAIN BOX */

.container{
  width:92%;
  max-width:430px;
  height:92vh;
  overflow-y:auto;
  background:rgba(255,255,255,0.35);
  backdrop-filter:blur(25px);
  border-radius:32px;
  border:1px solid rgba(255,255,255,0.45);
  padding:28px 22px 40px;
  z-index:2;
  box-shadow:0 15px 40px rgba(0,0,0,0.08);
}

.container::-webkit-scrollbar{
  width:0;
}

/* MOON */

.moon{
  width:120px;
  height:120px;
  border-radius:50%;
  background:linear-gradient(145deg,#fff,#ffeaf3);
  margin:auto;
  display:flex;
  justify-content:center;
  align-items:center;
  font-size:52px;
  animation:moonGlow 4s infinite alternate;
  box-shadow:0 10px 35px rgba(255,255,255,0.8);
}

@keyframes moonGlow{
  from{
    transform:scale(1);
  }

  to{
    transform:scale(1.05);
  }
}

h1{
  text-align:center;
  margin-top:22px;
  font-size:34px;
  color:#555;
}

.subtitle{
  margin-top:14px;
  text-align:center;
  color:#666;
  line-height:1.8;
  font-size:15px;
}

/* BREATHING */

.breathing{
  margin-top:35px;
  display:flex;
  flex-direction:column;
  align-items:center;
}

.circle{
  width:140px;
  height:140px;
  border-radius:50%;
  background:linear-gradient(145deg,#ffb9d5,#d7bfff);
  display:flex;
  justify-content:center;
  align-items:center;
  color:white;
  font-size:20px;
  animation:breathe 8s infinite ease-in-out;
  box-shadow:0 10px 30px rgba(255,185,213,0.4);
}

@keyframes breathe{
  0%{
    transform:scale(1);
  }

  50%{
    transform:scale(1.22);
  }

  100%{
    transform:scale(1);
  }
}

.breath-text{
  margin-top:18px;
  color:#666;
  font-size:14px;
  letter-spacing:1px;
}

/* CARDS */

.cards{
  margin-top:32px;
  display:flex;
  flex-direction:column;
  gap:16px;
}

.card{
  background:rgba(255,255,255,0.45);
  padding:18px;
  border-radius:22px;
  transition:0.4s;
  border:1px solid rgba(255,255,255,0.5);
}

.card:hover{
  transform:translateY(-4px);
}

.card h3{
  font-size:17px;
  margin-bottom:8px;
}

.card p{
  font-size:14px;
  line-height:1.7;
  color:#666;
}

/* BUTTON */

.music-btn{
  margin-top:28px;
  display:flex;
  justify-content:center;
}

button{
  border:none;
  padding:14px 24px;
  border-radius:40px;
  background:linear-gradient(145deg,#ffb8d3,#c9b9ff);
  color:white;
  font-size:14px;
  cursor:pointer;
  transition:0.3s;
  box-shadow:0 8px 20px rgba(201,185,255,0.4);
}

button:hover{
  transform:scale(1.05);
}

/* FOOTER */

.footer{
  margin-top:28px;
  text-align:center;
  font-size:13px;
  color:#777;
  font-style:italic;
  line-height:1.7;
}

</style>
</head>

<body>

<!-- BLURS -->

<div class="blur blur1"></div>
<div class="blur blur2"></div>

<!-- STARS -->

<div class="star" style="top:10%;left:20%"></div>
<div class="star" style="top:18%;left:75%"></div>
<div class="star" style="top:50%;left:12%"></div>
<div class="star" style="top:75%;left:85%"></div>
<div class="star" style="top:82%;left:30%"></div>

<!-- LOTUS -->

<div class="lotus lotus1">🪷</div>
<div class="lotus lotus2">🪷</div>

<!-- SUNFLOWERS -->

<div class="sunflower sunflower1">🌻</div>
<div class="sunflower sunflower2">🌻</div>

<!-- HEARTS -->

<div class="heart heart1">🧡</div>
<div class="heart heart2">🧡</div>
<div class="heart heart3">🧡</div>

<!-- FROGS -->

<div class="frog frog1">🐸</div>
<div class="frog frog2">🐸</div>
<div class="frog frog3">🐸</div>

<!-- MAIN -->

<div class="container">

  <div class="moon">🌙</div>

  <h1>Hey Likhitha 🌸</h1>

  <p class="subtitle">
    If your head hurts right now...
    <br>
    stay here quietly for a minute ☁️
    <br>
    breathe slowly with me.
  </p>

  <!-- BREATHING -->

  <div class="breathing">

    <div class="circle">
      Breathe
    </div>

    <div class="breath-text" id="breathText">
      Inhale Slowly...
    </div>

  </div>

  <!-- CARDS -->

  <div class="cards">

    <div class="card">
      <h3>🌸 Slow Down</h3>
      <p>
        You don’t have to fix everything tonight.
        Let your mind rest softly for a while.
      </p>
    </div>

    <div class="card">
      <h3>💧 Water Reminder</h3>
      <p>
        Drink a few sips of water slowly.
        Your body deserves care too.
      </p>
    </div>

    <div class="card">
      <h3>🐸 Tiny Frog Therapy</h3>
      <p>
        Frog says:
        things will feel softer soon 🌿
      </p>
    </div>

    <div class="card">
      <h3>🪷 Lotus Reminder</h3>
      <p>
        Even muddy water grows beautiful lotus flowers.
        Rest is beautiful too.
      </p>
    </div>

    <div class="card">
      <h3>🧡 For Likhitha</h3>
      <p>
        If your head hurts,
        stay here for a while.
        this tiny peaceful place just for you.
      </p>
    </div>

  </div>

  <!-- MUSIC -->

  <div class="music-btn">
    <button onclick="toggleMusic()">
      🎵 Play Calm Rain Sound
    </button>
  </div>

  <audio id="rainAudio" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_c8c8e56d1f.mp3?filename=rain-ambient-110397.mp3" type="audio/mp3">
  </audio>

  <!-- FOOTER -->

  <div class="footer">
    “A tiny peaceful corner made with care 🌸”
  </div>

</div>

<script>

const breathText = document.getElementById("breathText");

let inhale = true;

setInterval(()=>{

  if(inhale){
    breathText.innerText = "Exhale Gently...";
  }

  else{
    breathText.innerText = "Inhale Slowly...";
  }

  inhale = !inhale;

},4000);

const audio = document.getElementById("rainAudio");

let playing = false;

function toggleMusic(){

  const btn = event.target;

  if(!playing){

    audio.play();
    btn.innerText = "⏸ Pause Rain Sound";

  }

  else{

    audio.pause();
    btn.innerText = "🎵 Play Calm Rain Sound";

  }

  playing = !playing;
}

</script>

</body>
</html>
