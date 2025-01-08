<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Scrapbook untuk Salma</title>
  <style>
    /* Gaya Dasar */
    body, html {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      scroll-behavior: smooth;
    }

    section {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      font-size: 1.5em;
      color: white;
      position: relative;
      overflow: hidden;
      padding: 20px;
    }

    .parallax {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-size: cover;
      background-attachment: fixed;
      z-index: -1;
    }

    /* Latar untuk setiap halaman */
    #section1 .parallax { background: url('https://source.unsplash.com/random/1920x1080?nature') no-repeat center center; }
    #section2 .parallax { background: url('https://source.unsplash.com/random/1920x1080?flowers') no-repeat center center; }
    #section3 .parallax { background: url('https://source.unsplash.com/random/1920x1080?sky') no-repeat center center; }
    #section4 .parallax { background: url('https://source.unsplash.com/random/1920x1080?mountain') no-repeat center center; }
    #section5 .parallax { background: url('https://source.unsplash.com/random/1920x1080?city') no-repeat center center; }
    #section6 .parallax { background: url('https://source.unsplash.com/random/1920x1080?beach') no-repeat center center; }
    #section7 .parallax { background: url('https://source.unsplash.com/random/1920x1080?forest') no-repeat center center; }

    /* Warna Latar */
    #section1 { background: rgba(250, 21, 114, 0.4); }
    #section2 { background: rgba(250, 21, 115, 0.5); }
    #section3 { background: rgba(250, 21, 116, 0.6); }
    #section4 { background: rgba(250, 21, 117, 0.7); }
    #section5 { background: rgba(250, 21, 116, 0.5); }
    #section6 { background: rgba(250, 21, 115, 0.3); }
    #section7 { background: rgba(250, 21, 114, 0.6); }

    /* Tombol Scroll */
    .scrapbook-btn {
      padding: 15px 30px;
      font-size: 1.2em;
      background: rgba(255, 176, 255, 0.6);
      color: white;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }

    .scrapbook-btn:hover {
      background: rgba(25, 0, 0, 0.9);
    }

    /* Space untuk Tulisan */
    .text-content {
      background-color: rgba(0, 0, 0, 0.5);
      padding: 20px;
      border-radius: 10px;
      max-width: 80%;
      margin: 0 auto;
    }
  </style>
</head>
<body>

  <!-- Halaman 1 -->
  <section id="section1">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>Halo Najma Salma!</h1>
      <p>Aku panggil ama aja gapapa kan? halooww ama, gimana kabarnya?(jawab dalem hati juga gapapa) ciee tahun ini kepala dua hehe</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section2')">Bisa kamu scroll sih tapi saranku klik ini </button>
    </div>
  </section>

  <!-- Halaman 2 -->
  <section id="section2">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>Gimana Di UB?</h1>
      <p>Cieee di UB agak jauh juga ya ma, tapi seru di sana? aku tebak sih kayanya seru nich</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section3')">Kita lanjut dulu</button>
    </div>
  </section>

  <!-- Halaman 3 -->
  <section id="section3">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>Ini apa toh?</h1>
      <p>Mungkin kamu bingung? Ini apa toh? Udah liat isi dari bingkisanku? Nah anggap aja ini ucapanya(kalo pake tulis tangan, tulisanku jelek nanti kamu gak bisa bacanya</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section4')">lanjut dulu lagi yuk</button>
    </div>
  </section>

  <!-- Halaman 4 -->
  <section id="section4">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>Aku Suka Kamu</h1>
      <p>Aku tau ini aneh, tapi aku suka kamu. Tenang aja tapi ma, "aku suka kamu" atau "aku mencintaimu" anggap aja itu sebuah informasi untuk menambah wawasan pengetahuanmu</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section5')">Lanjut dulu lagi</button>
    </div>
  </section>

  <!-- Halaman 5 -->
  <section id="section5">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>"hmm si tyo aneh banget"</h1>
      <p>Biarlah itu jadi urusanku ma mengenai "aku suka kamu", bagaimana perasaanmu ke aku, biarlah itu jadi urusanmu. Toh kamu suka juga gak pantas aku disukai olehmu, yang pantas mah aku yang mencintaimu.</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section6')">Oke maaf buat ilfil tapi lanjut dulu</button>
    </div>
  </section>

  <!-- Halaman 6 -->
  <section id="section6">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>Setelahnya apa?</h1>
      <p>Nah buat mengakhiri ini, aku cuma mau bilang "Semangaatttt yaaaaaaa" aku gak tau pasti kamu sedih kenapa, galau kenapa, tapii semangatttt ama, kalo terjadi sesuatu yang bikin kamu down inget ini "Everything happens cause a reason, so let it flow"</p>
      <button class="scrapbook-btn" onclick="scrollToSection('section7')">Okee next itu part terakhir</button>
    </div>
  </section>

  <!-- Halaman 7 -->
  <section id="section7">
    <div class="parallax"></div>
    <div class="text-content">
      <h1>"Loh kaya gak asing?"</h1>
      <p>Hehe iya itu kalimatmu diyearbook. Dan terakhir, makasih ya udah luangin waktu buat baca ini, tulisan aneh ini. Gimana ke depannya nanti, tetap semangat gak sih ma, lancar kuliahmu, dan semoga apapun impian yang pengen kamu capai akhirnya tercapai.</p>
    </div>
  </section>

  <!-- Musik Latar -->
  <audio id="background-music" loop>
    <source src="Blue-Yung-Kai.mp3" type="audio/mpeg">
    Browsermu tidak mendukung elemen audio.
  </audio>

  <script>
    // Fungsi Scroll Halus ke Bagian
    function scrollToSection(sectionId) {
      document.getElementById(sectionId).scrollIntoView({ behavior: 'smooth' });
    }

    // Memainkan Musik Otomatis saat Scroll ke Section 2
    const music = document.getElementById('background-music');
    const section2 = document.getElementById('section2');

    window.addEventListener('scroll', () => {
      const section2Position = section2.getBoundingClientRect().top;
      if (section2Position <= window.innerHeight / 2 && music.paused) {
        music.play();
      }
    });
  </script>

</body>
</html>
