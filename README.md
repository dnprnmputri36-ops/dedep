[index.html](https://github.com/user-attachments/files/33202124/index.html)
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>From 2015, With Love — Yaya</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Caveat:wght@500;600;700&family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@600;700&display=swap');

:root{
  --cream:#fff9f0;
  --paper:#fffdf8;
  --ink:#493b45;
  --muted:#766a72;
  --pink:#f6a6b8;
  --coral:#f58f78;
  --yellow:#f7d66d;
  --blue:#9bd9df;
  --green:#acd9b7;
  --lilac:#c8b5e8;
  --line:#eadbd0;
}

*{
  box-sizing:border-box
}

html{
  scroll-behavior:smooth
}

body{
  margin:0;
  background:var(--cream);
  color:var(--ink);
  font-family:"DM Sans",sans-serif;
  line-height:1.7;
  overflow-x:hidden
}

h1,h2,h3{
  font-family:"Playfair Display",serif;
  line-height:1.15;
  margin:0
}

.script{
  font-family:"Caveat",cursive
}

.container{
  width:min(1080px,92%);
  margin:auto
}

section{
  padding:92px 0;
  position:relative
}

.eyebrow{
  font-size:.76rem;
  letter-spacing:.18em;
  text-transform:uppercase;
  font-weight:700;
  color:var(--muted);
  margin-bottom:12px
}

.section-title{
  font-size:clamp(2.2rem,5vw,4rem)
}

.section-intro{
  max-width:680px;
  color:var(--muted);
  margin:18px auto 0;
  text-align:center
}

.center{
  text-align:center
}

.paper{
  background:var(--paper);
  border:1px solid var(--line);
  box-shadow:0 14px 40px rgba(73,59,69,.08);
  border-radius:24px
}

.btn{
  display:inline-flex;
  align-items:center;
  gap:9px;
  padding:13px 20px;
  border:0;
  border-radius:999px;
  background:var(--ink);
  color:#fff;
  font-weight:700;
  cursor:pointer;
  transition:.25s;
  box-shadow:0 8px 20px rgba(73,59,69,.15)
}

.btn:hover{
  transform:translateY(-2px)
}

/* HERO */

.hero{
  min-height:100svh;
  display:grid;
  place-items:center;
  padding:40px 0;
  overflow:hidden
}

.hero:before,
.hero:after{
  content:"";
  position:absolute;
  border-radius:50%;
  opacity:.65
}

.hero:before{
  width:280px;
  height:280px;
  background:var(--pink);
  left:-110px;
  top:8%
}

.hero:after{
  width:330px;
  height:330px;
  background:var(--blue);
  right:-120px;
  bottom:2%
}

.hero-card{
  width:min(900px,92%);
  padding:54px 34px;
  text-align:center;
  position:relative;
  z-index:2
}

.hero h1{
  font-size:clamp(3.1rem,8vw,6.5rem);
  margin:8px 0 10px
}

.hero-sub{
  font-size:1.05rem;
  color:var(--muted);
  max-width:540px;
  margin:0 auto 30px
}

.envelope-wrap{
  margin:28px auto 24px;
  position:relative;
  width:210px;
  height:150px;
  cursor:pointer
}

.envelope{
  position:absolute;
  inset:0;
  background:#fff0f3;
  border:2px solid #e9b2bd;
  border-radius:10px;
  box-shadow:0 12px 25px rgba(73,59,69,.12)
}

.envelope:before{
  content:"";
  position:absolute;
  inset:0;
  background:
    linear-gradient(
      135deg,
      transparent 49%,
      #e9b2bd 50%,
      transparent 51%
    ),
    linear-gradient(
      225deg,
      transparent 49%,
      #e9b2bd 50%,
      transparent 51%
    );
  opacity:.8
}

.flap{
  position:absolute;
  left:0;
  top:0;
  width:100%;
  height:78px;
  background:#ffdbe3;
  clip-path:polygon(0 0,100% 0,50% 100%);
  transform-origin:top;
  transition:transform .8s;
  z-index:3
}

.envelope.open .flap{
  transform:rotateX(180deg)
}

.envelope-label{
  position:absolute;
  inset:42px 0 auto;
  text-align:center;
  z-index:4;
  font-family:Caveat;
  font-size:1.65rem
}

.hero-note{
  font-family:Caveat;
  font-size:1.4rem;
  transform:rotate(-2deg);
  display:inline-block;
  background:#fff5b9;
  padding:7px 18px;
  box-shadow:3px 4px 0 rgba(73,59,69,.08)
}

.scroll-hint{
  margin-top:25px;
  color:var(--muted);
  font-size:.85rem
}

/* TIMELINE */

.timeline{
  display:grid;
  gap:22px;
  max-width:760px;
  margin:42px auto
}

.timeline-item{
  display:grid;
  grid-template-columns:100px 1fr;
  gap:20px;
  align-items:start
}

.year{
  font-family:Caveat;
  font-size:2rem;
  font-weight:700;
  text-align:right
}

.timeline-card{
  padding:22px 25px;
  position:relative
}

.tape{
  position:absolute;
  width:70px;
  height:20px;
  top:-10px;
  left:30px;
  transform:rotate(-3deg);
  background:rgba(247,214,109,.65)
}

/* JIE JIE */

.jie-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:16px;
  margin-top:42px
}

.person{
  padding:24px 18px;
  text-align:center;
  min-height:190px;
  display:flex;
  flex-direction:column;
  justify-content:center
}

.person:nth-child(1){
  background:#e5f4e9
}

.person:nth-child(2){
  background:#ffe1d8
}

.person:nth-child(3){
  background:#e6f5f7
}

.person:nth-child(4){
  background:#eee8fa
}

.person .emoji{
  font-size:2.2rem
}

.person h3{
  font-size:1.45rem;
  margin:8px 0 4px
}

.person p{
  margin:0;
  color:var(--muted);
  font-size:.9rem
}

/* STORY */

.story{
  max-width:820px;
  margin:42px auto 0;
  padding:40px
}

.story p{
  margin:0 0 18px
}

.story p:last-child{
  margin-bottom:0
}

.highlight{
  background:
    linear-gradient(
      transparent 55%,
      #ffe88f 55%
    );
  font-weight:700
}

.quote{
  font-family:Caveat;
  font-size:2rem;
  line-height:1.25;
  text-align:center;
  margin:34px auto;
  max-width:700px
}

/* MAKNAE */

.maknae{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:28px;
  align-items:stretch;
  margin-top:42px
}

.maknae-card{
  padding:34px;
  position:relative;
  overflow:hidden
}

.maknae-card:first-child{
  background:#fff0f3
}

.maknae-card:last-child{
  background:#eef8f1
}

.sticker{
  display:inline-block;
  padding:6px 12px;
  border-radius:999px;
  font-weight:700;
  font-size:.78rem;
  background:#fff;
  transform:rotate(-3deg);
  box-shadow:0 4px 12px rgba(73,59,69,.08)
}

/* MEMORIES */

.memory-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
  margin-top:42px
}

.memory{
  padding:28px;
  min-height:240px;
  position:relative
}

.memory:nth-child(1){
  background:#fff2b8
}

.memory:nth-child(2){
  background:#ffdfe7
}

.memory:nth-child(3){
  background:#dff3f5
}

.memory:nth-child(4){
  background:#e4f3e7
}

.memory:nth-child(5){
  background:#eee6fa
}

.memory:nth-child(6){
  background:#ffe5d9
}

.memory .icon{
  font-size:2.2rem
}

.memory h3{
  font-size:1.45rem;
  margin:12px 0 7px
}

.memory p{
  font-size:.92rem;
  color:#62565d;
  margin:0
}

.memory small{
  display:block;
  margin-top:14px;
  color:#7c6c72;
  font-weight:700
}

/* NEW CHAPTER */

.newchapter{
  background:#f4eefa
}

.newchapter-card{
  padding:45px;
  max-width:800px;
  margin:40px auto
}

/* LETTER */

.letter-wrap{
  max-width:850px;
  margin:42px auto
}

.letter{
  padding:48px 52px;
  position:relative
}

.letter:before{
  content:"";
  position:absolute;
  inset:14px;
  border:1px dashed #e5d3c7;
  border-radius:18px;
  pointer-events:none
}

.letter-content{
  position:relative;
  z-index:1
}

.letter p{
  margin:0 0 18px
}

.letter h2{
  text-align:center;
  margin-bottom:28px;
  font-size:2.5rem
}

.letter-sign{
  text-align:right;
  font-family:Caveat;
  font-size:2rem;
  margin-top:30px
}

/* FINAL */

.final{
  min-height:85svh;
  display:grid;
  place-items:center;
  text-align:center;
  background:#fff4e8;
  overflow:hidden
}

.final .content{
  position:relative;
  z-index:2
}

.final h2{
  font-size:clamp(2.8rem,7vw,5.5rem);
  margin:12px 0 20px
}

.final-line{
  font-family:Caveat;
  font-size:2rem;
  max-width:700px;
  margin:0 auto 30px
}

.footer{
  padding:28px;
  text-align:center;
  color:var(--muted);
  font-size:.82rem
}

/* FLOATING ELEMENTS */

.float{
  position:absolute;
  font-size:2rem;
  animation:float 5s ease-in-out infinite
}

.f1{
  left:12%;
  top:16%
}

.f2{
  right:15%;
  top:20%;
  animation-delay:1s
}

.f3{
  left:17%;
  bottom:14%;
  animation-delay:2s
}

.f4{
  right:12%;
  bottom:12%;
  animation-delay:3s
}

@keyframes float{
  50%{
    transform:translateY(-13px) rotate(7deg)
  }
}

/* CONFETTI */

.confetti{
  position:fixed;
  inset:0;
  pointer-events:none;
  z-index:20;
  overflow:hidden
}

.confetti i{
  position:absolute;
  top:-20px;
  font-style:normal;
  font-size:1.3rem;
  animation:fall 3.2s linear forwards
}

@keyframes fall{
  to{
    transform:translateY(110vh) rotate(520deg);
    opacity:.1
  }
}

/* REVEAL */

.reveal{
  opacity:0;
  transform:translateY(22px);
  transition:.7s ease
}

.reveal.visible{
  opacity:1;
  transform:none
}

/* RESPONSIVE */

@media(max-width:760px){

  section{
    padding:68px 0
  }

  .hero-card{
    padding:40px 20px
  }

  .timeline-item{
    grid-template-columns:65px 1fr;
    gap:12px
  }

  .year{
    font-size:1.55rem
  }

  .jie-grid,
  .memory-grid{
    grid-template-columns:1fr 1fr
  }

  .maknae{
    grid-template-columns:1fr
  }

  .story,
  .letter,
  .newchapter-card{
    padding:28px 23px
  }

  .letter:before{
    inset:9px
  }
}

@media(max-width:480px){

  .jie-grid,
  .memory-grid{
    grid-template-columns:1fr
  }

  .envelope-wrap{
    width:185px;
    height:132px
  }
}

@media(prefers-reduced-motion:reduce){

  *,
  *:before,
  *:after{
    scroll-behavior:auto!important;
    animation:none!important;
    transition:none!important
  }
}
</style>
</head>

<body>

<div id="confetti" class="confetti"></div>

<!-- =========================
     HERO / OPENING
========================= -->

<section class="hero" id="top">

  <span class="float f1">🌸</span>
  <span class="float f2">🦋</span>
  <span class="float f3">🌼</span>
  <span class="float f4">✨</span>

  <div class="hero-card paper">

    <div class="eyebrow">
      A little letter from 2015 to your new chapter
    </div>

    <div class="hero-note">
      For Yaya ♡
    </div>

    <h1>
      From 2015,<br>
      With Love
    </h1>

    <p class="hero-sub">
      Before I say congratulations, I want to take you back
      for a little while — to where our story started.
    </p>

    <div class="envelope-wrap" id="envelope">

      <div class="envelope">

        <div class="flap"></div>

        <div class="envelope-label">
          open me ♡
        </div>

      </div>

    </div>

    <button class="btn" id="openBtn">
      Open our story →
    </button>

    <div class="scroll-hint">
      A small trip down memory lane
    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 01
========================= -->

<section id="2015">

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 01
      </div>

      <h2 class="section-title">
        Back to 2015
      </h2>

      <p class="section-intro">
        Before wedding dresses, new homes, and grown-up decisions —
        there were four high school girls simply trying to figure out life.
      </p>

    </div>


    <div class="timeline">

      <div class="timeline-item reveal">

        <div class="year">
          2015
        </div>

        <div class="paper timeline-card">

          <span class="tape"></span>

          <h3>
            It started with two pairs of seatmates.
          </h3>

          <p>
            Uswa with Dian, then Pedep with Yaya.
            We were not even a fixed group of four.
            Somehow, we just found our way to become
            <b>Jie Jie</b>.
          </p>

        </div>

      </div>


      <div class="timeline-item reveal">

        <div class="year">
          SMA
        </div>

        <div class="paper timeline-card">

          <h3>
            And somehow, we stayed.
          </h3>

          <p>
            We were busy dreaming about which major,
            which campus, and what kind of future we wanted.
            We did not know then that this friendship would
            travel much further than high school.
          </p>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 02
========================= -->

<section id="jie-jie" style="background:#fff4ea">

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 02
      </div>

      <h2 class="section-title">
        Jie Jie — Our Little Chaos
      </h2>

      <p class="section-intro">
        Four people. Four personalities.
        One friendship that somehow made perfect sense.
      </p>

    </div>


    <div class="jie-grid reveal">

      <div class="paper person">

        <div class="emoji">
          🌿
        </div>

        <h3>
          Dian
        </h3>

        <p>
          The wise one.
        </p>

      </div>


      <div class="paper person">

        <div class="emoji">
          💥
        </div>

        <h3>
          Uswa
        </h3>

        <p>
          The explosive one.
        </p>

      </div>


      <div class="paper person">

        <div class="emoji">
          🍵
        </div>

        <h3>
          Yaya
        </h3>

        <p>
          The favorite target.
        </p>

      </div>


      <div class="paper person">

        <div class="emoji">
          😈
        </div>

        <h3>
          Pedep
        </h3>

        <p>
          The tengil one.
        </p>

      </div>

    </div>


    <div class="story paper reveal">

      <p>
        Kalau saya harus menggambarkan Jie Jie,
        mungkin satu kata yang paling tepat adalah:
          campur aduk, tapi mantap.
        </span>
      </p>

      <p>
        Ada Dian yang bijaksana, Uswa yang meledak-ledak,
        Yaya yang entah bagaimana paling sering menjadi target
        bahan candaan, dan saya yang tengil serta selalu punya saja
        bahan untuk membully Yaya.
      </p>

      <p>
        Empat orang dengan karakter yang mungkin kalau dipikir-pikir
        tidak masuk akal kalau disatukan.
        Tapi justru itu yang membuat Jie Jie menjadi Jie Jie.
        #ea
      </p>

      <p>
        Dulu, waktu SMA, tak pernah terbayangkan kalau kita bakal
        berteman selama ini.
        Semuanya dimulai dari duduk sebangku,
        Uswa dengan Dian, lalu saya dengan Yaya.
        Kita sebenarnya bukan <i>fixed group</i> berempat,
        tapi anehnya, kita menemukan jalan untuk menyatu.
      </p>

      <p>
        Kita kemudian masuk ke dunia perkuliahan yang carut-marut
        dengan jalan masing-masing.
        Empat orang, empat jurusan, empat kehidupan yang perlahan
        berjalan ke arah yang berbeda.
      </p>

      <p>
        Sampai akhirnya datang masa skripsi.
      </p>

      <p>
        Dan rasanya seperti perang.
      </p>

      <p>
        Masing-masing dari kita punya medan perang sendiri.
        Ada hari ketika kita pusing dengan revisi,
        kehilangan arah, merasa tertinggal,
        atau hanya ingin semuanya cepat selesai.
      </p>

      <p>
        Tapi mungkin memang ada alasan kenapa Tuhan
        mempertemukan kita sejak SMA.
      </p>

      <p>
        Kali ini bukan lagi sekadar teman sebangku.
      </p>

      <p>
        Bukan lagi hanya sekumpulan anak SMA yang bercanda bersama.
      </p>

      <p>
        Tapi empat orang yang saling menguatkan
        untuk memenangkan perang masing-masing.
      </p>

      <p>
        Dan kalau sekarang saya melihat ke belakang,
        rasanya lucu juga.
      </p>

      <p>
        Kita mungkin tidak memenangkan semua pertempuran
        dengan cara yang sama.
        Tapi setidaknya kita tahu bahwa selama masa-masa itu,
        kita tidak benar-benar sendirian.
      </p>

    </div>


    <div class="quote reveal">
      “God brought us together in high school,
      and somehow brought us back together
      when we needed each other most.”
    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 03
========================= -->

<section id="maknae">

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 03
      </div>

      <h2 class="section-title">
        For Yaya — Our Little Maknae
      </h2>

      <p class="section-intro">
        The youngest one. The shy one.
        The one we teased the most — and loved just as much.
      </p>

    </div>


    <div class="maknae">

      <div class="paper maknae-card reveal">

        <span class="sticker">
          SI PECA'
        </span>

        <h3 style="font-size:2rem;margin:18px 0 15px">
          Our little sister
        </h3>

        <p>
          Kalau dipikir-pikir, di antara kita berempat,
          kamu itu memang kayak adek kecil.
        </p>

        <p>
          Maknae-nya Jie Jie.
        </p>

        <p>
          Mungkin karena kamu memang anak bungsu,
          jadi sifat adeknya makin terasa. 
        </p>

        <p>
          Dulu waktu SMA, kami bahkan suka panggil kamu
          Peca', karena menurut kami kamu itu lemah sekali.
          Wkwk.
        </p>

        <p>
          Sampai sekarang saya masih suka memperagakan cara kamu
          melakukan roll depan yang entah bagaimana selalu gagal.
        </p>

        <p>
          Terus kalau sudah malu, muka kamu akan merah
          seperti kepiting rebus. 🦀
        </p>

        <p>
          Makanya lahirlah satu panggilan lagi:
          Humairah — yang berpipi merah.
        </p>

        <p>
          Lucunya, badanmu justru paling tinggi di antara kita berempat.
          Tapi kalau soal nyali?
        </p>

        <p>
          Paling imut.
        </p>

      </div>


      <div class="paper maknae-card reveal">

        <span class="sticker">
          BRAVE YAYA
        </span>

        <h3 style="font-size:2rem;margin:18px 0 15px">
          More brave than she thinks
        </h3>

        <p>
          Kamu punya banyak sekali ketakutan.
          Tapi semakin dewasa, saya justru sadar bahwa rasa takut
          itu tidak pernah benar-benar membuatmu berhenti.
        </p>

        <p>
          Di balik Yaya yang pemalu, gampang tersipu,
          banyak takutnya, dan sering jadi bahan bully-an kami,
          ternyata ada seseorang yang akan memperjuangkan
          apa yang benar-benar dia inginkan.
        </p>

        <p>
          Perjalananmu dengan Miftah adalah salah satu contohnya.
          Kamu berdoa, mencari petunjuk, dan ketika hatimu
          tidak condong pada perjodohan itu, kamu tetap memilih
          untuk mengusahakan Miftah dengan caramu sendiri.
        </p>

        <p>
            Kamu tidak harus menjadi orang yang tidak punya rasa takut
            untuk menjadi berani.
        </p>

        <p>
          Kadang keberanian itu justru berarti tetap melangkah
          meskipun kita takut.
        </p>

      </div>

    </div>


    <div class="quote reveal">
      “Si Peca' yang dulu roll depannya selalu gagal itu…
      sekarang sudah sampai sejauh ini.”
    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 04
========================= -->

<section id="memories" style="background:#fff7ec">

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 04
      </div>

      <h2 class="section-title">
        The Little Things I Remember
      </h2>

      <p class="section-intro">
        The memories that may look small from the outside,
        but somehow became the things I know I will always remember.
      </p>

    </div>


    <div class="memory-grid">

      <article class="paper memory reveal">

        <div class="icon">
          🍵
        </div>

        <h3>
          The Tea Ritual
        </h3>

        <p>
          Yaya memulai pagi dengan teh.
          Tea holic sejati.
          Some things are simply non-negotiable.
        </p>

      </article>


      <article class="paper memory reveal">

        <div class="icon">
          ⚽
        </div>

        <h3>
          Timnas Nights
        </h3>

        <p>
          Nobar di rumah Yaya, kadang sampai pagi.
          Kalau Indonesia menang, rasanya seperti kita yang
          memenangkan pertandingan.
        </p>

      </article>


      <article class="paper memory reveal">

        <div class="icon">
          🍳
        </div>

        <h3>
          After-Nobar Breakfast
        </h3>

        <p>
          Setelah begadang, lanjut sarapan.
          Kadang malah lanjut masak untuk makan siang.
          Somehow, that was enough.
        </p>

      </article>


      <article class="paper memory reveal">

        <div class="icon">
          🤸‍♀️
        </div>

        <h3>
          The Roll
        </h3>

        <p>
          Ada banyak hal memalukan yang bisa diceritakan tentang Yaya.
          Tapi tetap saja:
          Yaya tidak bisa roll depan. 😂
        </p>

      </article>


      <article class="paper memory reveal">

        <div class="icon">
          🍗
        </div>

        <h3>
          Only Chicken Breast
        </h3>

        <p>
          Yaya tidak bisa makan ayam kalau bukan bagian dada.
          Tidak ada kompromi.
          Dada ayam atau tidak sama sekali.
        </p>

      </article>


      <article class="paper memory reveal">

        <div class="icon">
          💥
        </div>

        <h3>
          That Chaotic Day
        </h3>

        <p>
          Uswa selesai seminar akhir,
          kita mau menyambangi Dian yang juga seminar akhir.
          Lalu di perjalanan pulang, jari Yaya mulai nyut-nyutan
          dan semakin lama semakin sakit buat kita semua khawatir wkwk 
        </p>

      </article>

    </div>


    <div
      class="story paper reveal"
      style="margin-top:28px"
    >

      <p>
        Dan tentu saja ada malam-malam di rumah Yaya:
        kumpul, nobar, ngobrol sampai pagi, sarapan,
        kadang masak untuk makan siang.
        Tidak selalu ada sesuatu yang besar terjadi.
      </p>

      <p>
        Tapi mungkin justru itu yang membuatnya berharga.
      </p>

      <p>
        Begitulah Jie Jie.
        Tidak selalu punya cerita besar.
        Tidak selalu punya rencana.
        Tapi selalu berhasil pulang membawa kenangan.
      </p>

    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 05
========================= -->

<section
  class="newchapter"
  id="newchapter"
>

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 05
      </div>

      <h2 class="section-title">
        And Then, A New Chapter
      </h2>

      <p class="section-intro">
        A chapter I may not know every detail of,
        but one I am very happy to see you begin.
      </p>

    </div>


    <div class="paper newchapter-card reveal">

      <p>
        Saya mungkin tidak tahu seluruh cerita tentang bagaimana
        kalian sampai di titik ini.
      </p>

      <p>
        Saya tidak ada di setiap percakapan kalian,
        tidak tahu semua proses yang kalian lewati,
        dan mungkin tidak akan pernah tahu seluruh cerita
        di balik keputusan kalian untuk akhirnya berjalan bersama.
      </p>

      <p>
        Tapi saya tahu satu hal.
      </p>

      <p>
        Saya tahu Yaya pernah berdoa.
        Saya tahu Yaya pernah berada dalam kebingungan.
        Dan saya tahu, ketika akhirnya hatinya menemukan arah,
        Yaya memilih untuk mengusahakannya dengan caranya sendiri.
      </p>

      <p>
        Hari ini, jalan itu membawa Yaya sampai kepada Miftah.
      </p>

      <p>
        Dan sekarang, kalian akan memulai perjalanan yang baru.
      </p>

      <p>
        Semoga setelah ini kalian bukan hanya menjadi pasangan
        dalam keadaan mudah, tetapi juga menjadi tempat pulang
        ketika hidup sedang tidak mudah.
      </p>

      <p>
        Semoga kalian bisa saling mengingatkan,
        saling menguatkan,
        dan saling membawa lebih dekat kepada Allah.
      </p>

      <p>
        <b>
          Selamat menempuh perjalanan baru,
          Yaya dan Miftah. 🤍
        </b>
      </p>

    </div>

  </div>

</section>


<!-- =========================
     CHAPTER 06 — LETTER
========================= -->

<section id="letter">

  <div class="container">

    <div class="center reveal">

      <div class="eyebrow">
        Chapter 06
      </div>

      <h2 class="section-title">
        A Letter From Dedep
      </h2>

      <p class="section-intro">
        For the girl who started as my seatmate
        and became one of the people I am most grateful
        to have in my life.
      </p>

    </div>


    <div class="letter-wrap reveal">

      <div class="paper letter">

        <div class="letter-content">

          <h2>
            For Yaya ♡
          </h2>

          <p>
            Yaya,
          </p>

          <p>
            Sampai sekarang saya masih merasa agak aneh
            membayangkan kamu menikah.
          </p>

          <p>
            Waktu pertama kali tahu, rasanya banyak sekali
            yang datang bersamaan.
            Kaget, sedih, senang, lega—semuanya campur aduk.
          </p>

          <p>
            Senang karena akhirnya kamu akan bersama seseorang
            yang selama ini kamu doakan.
          </p>

          <p>
            Lega karena akhirnya kamu tidak perlu lagi pusing
            dengan perjodohan itu.
          </p>

          <p>
            Tapi di sisi lain, ada sedikit rasa sedih juga.
            Karena tiba-tiba saya sadar bahwa teman kami
            akan membangun keluarganya sendiri.
          </p>

          <p>
            Mungkin setelah ini kita tidak akan sebebas dulu
            untuk sekadar menginap, berkumpul sampai pagi,
            nobar, masak-masak, atau melakukan hal-hal random
            seperti dulu terlebih ada jarak yang membentang
          </p>

          <p>
            Dan ternyata, tumbuh dewasa memang seperti ini ya.
          </p>

          <p>
            Orang-orang yang kita sayangi perlahan memasuki
            babak hidup mereka masing-masing.
          </p>

          <p>
            Tapi kalau ada satu hal yang paling saya syukuri
            dari persahabatan kita, itu adalah bagaimana kita
            bisa menjadi diri sendiri tanpa perlu takut dihakimi.
          </p>

          <p>
            Saya bisa menjadi Pedep yang tengil,
            banyak bercanda, dan kadang suka membully kamu. 
          </p>

          <p>
            Dan kamu bisa menjadi Yaya yang pemalu,
            banyak takutnya, banyak khawatirnya. 
            Si Peca' yang roll depannya selalu gagal,
            si Humairah yang mukanya merah kalau malu,
            dan tentu saja si picky eater yang kami suka gemas.
          </p>

          <p>
            Tapi lebih dari semua itu,
            saya bersyukur karena ada kamu sebagai teman.
          </p>

          <p>
            Ada kamu yang bisa menjadi pengingat
            ketika saya melakukan sesuatu yang salah.
          </p>

          <p>
            Ada kamu yang ikhlas membimbing 
            ketika saya lagi bingung.
          </p>

          <p>
            Dan ada kamu yang hadir ketika
            lelah dengan dunia,
            kalut tidak tahu harus bagaimana.
          </p>

          <p>
            Mungkin kamu tidak selalu sadar seberapa berarti
            kehadiranmu di hidupku.
          </p>

          <p>
            Tapi saya ingat.
          </p>

          <p>
            Saya ingat semuanya.
          </p>

          <p>
            Dan tanggal 26 Oktober nanti, ketika kamu memulai kehidupan baru
            bersama Miftah, saya ingin mendoakan:
          </p>

          <p>
            Semoga pernikahan kalian menjadi pernikahan yang
            sakinah, mawaddah, warahmah.
          </p>

          <p>
            Semoga kamu dan Miftah selalu dilimpahkan kebahagiaan.
          </p>

          <p>
            Semoga kalian selalu diberikan petunjuk ketika
            tidak tahu harus melangkah ke mana,
            diberikan kesabaran ketika keadaan tidak mudah,
            dan diberikan kemudahan dalam menjalankan
            ibadah terpanjang ini.
          </p>

          <p>
            Semoga rumah yang kalian bangun nantinya bukan hanya
            menjadi tempat untuk pulang, tetapi juga menjadi
            tempat di mana kalian berdua merasa aman,
            dicintai, dan selalu ingin kembali.
          </p>

          <p>
            Dan Yaya...
          </p>

          <p>
            Walaupun sekarang sudah ada Miftah,
            jangan lupakan kami.
          </p>

          <p>
            Kalau suatu hari kamu ingin cerita,
            ingin mengeluh, ingin tertawa,
            atau sekadar ingin kembali menjadi Yaya yang dulu,
            you can always come to me.
          </p>

          <p>
            Jarak mungkin membuat kita tidak bisa sesering
            dulu bertemu.
          </p>

          <p>
            Kehidupan mungkin akan membuat kita semakin sibuk.
          </p>

          <p>
            Dan mungkin nanti ada banyak hal yang berubah.
          </p>

          <p>
            Tapi saya harap satu hal tidak berubah:
          </p>

          <p>
            Kamu tetap tahu bahwa kamu punya kami.
          </p>

          <p>
            Dan meskipun saya tidak bisa hadir di sana
            untuk melihat langsung kamu berjalan menuju
            kehidupan barumu, ketahuilah, Yaya
          </p>

          <p>
              saya tidak hadir secara fisik,
              tapi doaku selalu menyertaimu.
          </p>

          <p>
            Selamat menikah, Yaya.
          </p>

          <p>
            Selamat memulai perjalanan baru bersama Miftah.
          </p>

          <p>
            Dari teman sebangku, teman seperjuangan,
            teman satu geng, sampai akhirnya melihat kamu
            menjadi seorang istri.
          </p>


          <div class="letter-sign">
            With all my love,<br>
            Dedep 🤍
          </div>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- =========================
     FINAL
========================= -->

<section
  class="final"
  id="final"
>

  <span class="float f1">🌷</span>
  <span class="float f2">💗</span>
  <span class="float f3">🦋</span>
  <span class="float f4">🌼</span>

  <div class="content reveal">

    <div class="eyebrow">
      And finally...
    </div>

    <h2>
      Yaya & Miftah
    </h2>

    <div class="final-line">
      Yaya, saya nda bisa hadir.
      Tapi doaku selalu menyertaimu.
    </div>

    <p
      style="
        max-width:650px;
        margin:0 auto 25px;
        color:var(--muted)
      "
    >
      Distance may keep me from being there today,
      but it could never keep me from celebrating you.
    </p>

    <button
      class="btn"
      onclick="celebrate()"
    >
      Congratulations ♡
    </button>

    <p
      class="script"
      style="
        font-size:1.7rem;
        margin-top:22px
      "
    >
      From your forever seatmate, Dedep
    </p>

  </div>

</section>


<div class="footer">
  Made with love, memories, and a little bit of Jie Jie chaos. ♡
</div>


<!-- =========================
     JAVASCRIPT
========================= -->

<script>

const envelope =
  document.getElementById('envelope');

const openBtn =
  document.getElementById('openBtn');


function openStory(){

  envelope
    .querySelector('.envelope')
    .classList.add('open');

  celebrate();

  setTimeout(() => {

    document
      .getElementById('2015')
      .scrollIntoView({
        behavior:'smooth'
      });

  },650);

}


envelope.onclick = openStory;

openBtn.onclick = openStory;


function celebrate(){

  const h =
    document.getElementById('confetti');

  const s = [
    '🌸',
    '🌷',
    '✨',
    '💗',
    '🌼',
    '🦋',
    '♡',
    '🌈'
  ];


  for(let i=0;i<38;i++){

    let e =
      document.createElement('i');

    e.textContent =
      s[Math.floor(Math.random()*s.length)];

    e.style.left =
      Math.random()*100+'vw';

    e.style.animationDelay =
      Math.random()*.7+'s';

    e.style.fontSize =
      .8+Math.random()*1.1+'rem';

    h.appendChild(e);

    setTimeout(
      () => e.remove(),
      4000
    );

  }

}


const observer =
  new IntersectionObserver(

    es => es.forEach(e => {

      if(e.isIntersecting){

        e.target.classList.add('visible');

      }

    }),

    {
      threshold:.12
    }

  );


document
  .querySelectorAll('.reveal')
  .forEach(e =>
    observer.observe(e)
  );

</script>

</body>
</html>
