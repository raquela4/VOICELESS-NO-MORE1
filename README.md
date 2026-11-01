
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#101722">
<meta name="description" content="VOICELESS NO MORE؛ پروژه‌ای مستقل برای حمایت از قربانیان، آگاهی‌رسانی و مطالبه عدالت.">
<title>VOICELESS NO MORE | صدای بی‌صداها</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700;800&display=swap');

:root {
  --bg: #101722;
  --bg2: #151f2c;
  --card: #1b2736;
  --blue: #718da9;
  --gold: #c7ad82;
  --white: #f0f1f3;
  --muted: #a2adba;
  --border: rgba(255,255,255,.09);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
  scroll-padding-top: 90px;
}

body {
  font-family: 'Vazirmatn', sans-serif;
  background: var(--bg);
  color: var(--white);
  line-height: 2;
}

a {
  color: inherit;
  text-decoration: none;
}

button {
  font-family: inherit;
  cursor: pointer;
}

.container {
  width: min(1120px, 90%);
  margin: auto;
}

/* HEADER */

header {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(16,23,34,.95);
  backdrop-filter: blur(14px);
  border-bottom: 1px solid var(--border);
}

.nav {
  height: 76px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 19px;
  font-weight: 800;
  letter-spacing: 1px;
  direction: ltr;
  color: var(--gold);
}

.logo span {
  display: block;
  font-size: 10px;
  color: var(--muted);
  letter-spacing: 3px;
  text-align: center;
}

.nav-links {
  display: flex;
  gap: 25px;
  align-items: center;
  font-size: 13px;
  color: var(--muted);
}

.nav-links a:hover {
  color: var(--gold);
}

.menu-btn {
  display: none;
  background: none;
  color: white;
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 7px 12px;
  font-size: 20px;
}

/* HERO */

.hero {
  min-height: 610px;
  display: flex;
  align-items: center;
  position: relative;
  overflow: hidden;
  background:
    linear-gradient(90deg, rgba(16,23,34,.35), #101722 95%),
    linear-gradient(0deg, #101722 0%, transparent 60%),
    url('https://images.unsplash.com/photo-1519608487953-e999c86e7455?auto=format&fit=crop&w=1800&q=85')
    center/cover;
}

.hero-content {
  max-width: 700px;
  padding: 90px 0;
  position: relative;
  z-index: 2;
}

.eyebrow {
  color: var(--gold);
  font-size: 12px;
  letter-spacing: 2px;
  margin-bottom: 20px;
}

.hero h1 {
  font-size: clamp(34px, 6vw, 66px);
  line-height: 1.5;
  font-weight: 800;
  margin-bottom: 20px;
}

.hero h1 span {
  color: var(--gold);
}

.hero p {
  max-width: 560px;
  color: #c2cad4;
  font-size: 15px;
  line-height: 2.3;
}

.hero-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 32px;
}

.btn {
  display: inline-block;
  padding: 11px 25px;
  border-radius: 7px;
  font-size: 13px;
  transition: .25s;
}

.btn-primary {
  background: var(--gold);
  color: #18202b;
  font-weight: 700;
}

.btn-primary:hover {
  background: #e2cda8;
  transform: translateY(-3px);
}

.btn-outline {
  border: 1px solid rgba(255,255,255,.35);
  color: white;
}

.btn-outline:hover {
  background: white;
  color: var(--bg);
}

/* GENERAL SECTIONS */

section {
  padding: 90px 0;
}

.section-heading {
  margin-bottom: 38px;
}

.section-heading small {
  color: var(--gold);
  font-size: 12px;
  letter-spacing: 1px;
}

.section-heading h2 {
  font-size: clamp(24px,4vw,35px);
  margin: 10px 0;
}

.section-heading p {
  color: var(--muted);
  font-size: 14px;
  max-width: 650px;
}

.about {
  background: var(--bg2);
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: center;
}

.about-image {
  min-height: 360px;
  border-radius: 12px;
  background:
    linear-gradient(0deg, rgba(16,23,34,.4), transparent),
    url('https://images.unsplash.com/photo-1532629345422-7515f3d16bb6?auto=format&fit=crop&w=1000&q=85')
    center/cover;
}

.about-text p {
  color: var(--muted);
  font-size: 14px;
  margin: 16px 0;
}

/* CARDS */

.cards {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 20px;
}

.card {
  background: var(--card);
  border: 1px solid var(--border);
  padding: 27px;
  border-radius: 12px;
  transition: .3s;
}

.card:hover {
  transform: translateY(-6px);
  border-color: var(--gold);
}

.card-icon {
  font-size: 28px;
  margin-bottom: 14px;
}

.card h3 {
  font-size: 17px;
  margin-bottom: 10px;
}

.card p {
  font-size: 13px;
  color: var(--muted);
  line-height: 2.2;
}

/* MESSAGE */

.quote-section {
  background:
    linear-gradient(rgba(15,23,35,.91),rgba(15,23,35,.96)),
    url('https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=1600&q=85')
    center/cover;
  text-align: center;
  padding: 100px 20px;
}

.quote-section h2 {
  color: var(--gold);
  font-size: clamp(25px,4vw,39px);
  margin-bottom: 20px;
}

.quote-section p {
  max-width: 650px;
  margin: auto;
  color: #d0d7df;
  font-size: 14px;
}

/* RESOURCES */

.resource-list {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 15px;
}

.resource {
  background: var(--card);
  padding: 22px;
  border-radius: 10px;
  border-right: 3px solid var(--blue);
}

.resource h3 {
  font-size: 15px;
  margin-bottom: 8px;
}

.resource p {
  color: var(--muted);
  font-size: 13px;
}

/* STORIES */

.story-note {
  background: #1c2a39;
  padding: 25px;
  border-radius: 10px;
  border: 1px solid var(--border);
}

.story-note p {
  color: var(--muted);
  font-size: 14px;
}

/* FOOTER */

footer {
  background: #0b111a;
  border-top: 1px solid var(--border);
  padding: 45px 0 20px;
}

.footer-grid {
  display: grid;
  grid-template-columns: 1.5fr 1fr 1fr;
  gap: 35px;
}

footer h3 {
  color: var(--gold);
  font-size: 15px;
  margin-bottom: 15px;
}

footer p, footer a {
  color: var(--muted);
  font-size: 12px;
}

footer a {
  display: block;
  margin: 7px 0;
}

footer a:hover {
  color: var(--gold);
}

.copyright {
  text-align: center;
  border-top: 1px solid var(--border);
  margin-top: 35px;
  padding-top: 18px;
  font-size: 11px;
  color: #758293;
}

/* MOBILE */

@media(max-width:800px) {
  .menu-btn {
    display: block;
  }

  .nav-links {
    display: none;
    position: absolute;
    top: 76px;
    right: 0;
    left: 0;
    background: #151f2c;
    padding: 20px 5%;
    flex-direction: column;
    align-items: stretch;
    gap: 15px;
    border-bottom: 1px solid var(--border);
  }

  .nav-links.open {
    display: flex;
  }

  .hero {
    min-height: 540px;
    background-position: 55% center;
  }

  .about-grid {
    grid-template-columns: 1fr;
    gap: 25px;
  }

  .about-image {
    min-height: 260px;
  }

  .cards {
    grid-template-columns: 1fr 1fr;
  }

  .footer-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media(max-width:520px) {
  section {
    padding: 65px 0;
  }

  .cards,
  .resource-list,
  .footer-grid {
    grid-template-columns: 1fr;
  }

  .hero h1 {
    font-size: 34px;
  }

  .hero p {
    font-size: 13px;
  }

  .logo {
    font-size: 16px;
  }
}
</style>
</head>

<body>

<header>
  <div class="container nav">

    <a href="#home" class="logo">
      VOICELESS NO MORE
      <span>THE VOICE OF JUSTICE</span>
    </a>

    <button class="menu-btn" id="menuBtn"
      aria-label="باز کردن منو" aria-expanded="false">☰</button>

    <nav class="nav-links" id="navLinks">
      <a href="#home">صفحه اصلی</a>
      <a href="#about">درباره ما</a>
      <a href="#support">حمایت</a>
      <a href="#rights">حقوق و آگاهی</a>
      <a href="#stories">داستان‌ها</a>
      <a href="#contact">ارتباط با ما</a>
    </nav>

  </div>
</header>

<!-- HERO -->

<main>

<section class="hero" id="home">
  <div class="container hero-content">

    <div class="eyebrow">
      VOICELESS NO MORE — IRAN
    </div>

    <h1>
      سکوت، پایان<br>
      <span>داستان نیست.</span>
    </h1>

    <p>
      ما برای جهانی تلاش می‌کنیم که در آن هیچ قربانی‌ای
      فراموش نشود، هیچ صدایی نادیده گرفته نشود و
      هیچ انسانی برای دریافت حمایت تنها نماند.
    </p>

    <div class="hero-buttons">
      <a href="#about" class="btn btn-primary">
        آشنایی با مأموریت ما
      </a>

      <a href="#support" class="btn btn-outline">
        راهنمای دریافت حمایت
      </a>
    </div>

  </div>
</section>

<!-- ABOUT -->

<section class="about" id="about">
  <div class="container about-grid">

    <div class="about-image"></div>

    <div class="about-text">

      <div class="section-heading">
        <small>WHO WE ARE</small>
        <h2>ما چه کسانی هستیم؟</h2>
      </div>

      <p>
        VOICELESS NO MORE یک پروژه مستقل آگاهی‌رسانی
        و حمایت از قربانیان آسیب‌های اجتماعی است.
      </p>

      <p>
        هدف ما ایجاد فضایی برای شناخت حقوق افراد آسیب‌دیده،
        معرفی مسیرهای دریافت حمایت و افزایش آگاهی عمومی
        درباره خشونت و بی‌عدالتی است.
      </p>

      <p>
        ما معتقدیم حمایت از قربانیان باید با احترام،
        حفظ حریم خصوصی و بدون قضاوت همراه باشد.
      </p>

    </div>
  </div>
</section>

<!-- MISSION -->

<section id="mission">
  <div class="container">

    <div class="section-heading">
      <small>OUR MISSION</small>
      <h2>برای چه چیزی تلاش می‌کنیم؟</h2>
      <p>
        سه اصل اساسی که مسیر فعالیت این پروژه را مشخص می‌کنند.
      </p>
    </div>

    <div class="cards">

      <article class="card">
        <div class="card-icon">♡</div>
        <h3>حمایت از قربانیان</h3>
        <p>
          معرفی راه‌های دریافت حمایت روان‌شناختی،
          اجتماعی و حقوقی برای افراد آسیب‌دیده.
        </p>
      </article>

      <article class="card">
        <div class="card-icon">⚖</div>
        <h3>مطالبه عدالت</h3>
        <p>
          ترویج آگاهی درباره حقوق افراد،
          پاسخ‌گویی نهادهای مسئول و اهمیت رسیدگی قانونی.
        </p>
      </article>

      <article class="card">
        <div class="card-icon">◉</div>
        <h3>آگاهی‌رسانی</h3>
        <p>
          شناخت انواع خشونت و سوءاستفاده،
          پیشگیری از آسیب و مقابله با عادی‌سازی آن.
        </p>
      </article>

    </div>
  </div>
</section>

<!-- QUOTE -->

<section class="quote-section">
  <div class="container">

    <h2>صدای تو اهمیت دارد.</h2>

    <p>
      هیچ انسانی نباید به دلیل ترس، شرم یا قضاوت دیگران
      مجبور به سکوت درباره آسیب‌هایی شود که تجربه کرده است.
      شنیده شدن، آغاز مسیر حمایت است.
    </p>

  </div>
</section>

<!-- SUPPORT -->

<section id="support">
  <div class="container">

    <div class="section-heading">
      <small>SUPPORT & CARE</small>
      <h2>حمایت از قربانیان</h2>
      <p>
        دریافت کمک حق توست. لازم نیست برای درخواست حمایت
        احساس شرم یا گناه داشته باشی.
      </p>
    </div>

    <div class="cards">

      <article class="card">
        <div class="card-icon">♡</div>
        <h3>حمایت روان‌شناختی</h3>
        <p>
          صحبت با روان‌شناس متخصص و دریافت حمایت عاطفی
          می‌تواند بخشی از مسیر بهبود باشد.
        </p>
      </article>

      <article class="card">
        <div class="card-icon">⚖</div>
        <h3>حمایت حقوقی</h3>
        <p>
          برای شناخت حقوق و گزینه‌های قانونی،
          از وکیل یا مشاور حقوقی معتبر کمک بگیر.
        </p>
      </article>

      <article class="card">
        <div class="card-icon">✦</div>
        <h3>حمایت اجتماعی</h3>
        <p>
          ارتباط با افراد امن، خانواده قابل اعتماد
          و مراکز حمایتی می‌تواند به کاهش احساس تنهایی کمک کند.
        </p>
      </article>

    </div>

  </div>
</section>

<!-- RIGHTS -->

<section id="rights" class="about">
  <div class="container">

    <div class="section-heading">
      <small>KNOW YOUR RIGHTS</small>
      <h2>آگاهی، نخستین قدم است.</h2>
      <p>
        شناخت حقوق و راه‌های دریافت کمک،
        امکان تصمیم‌گیری آگاهانه را فراهم می‌کند.
      </p>
    </div>

    <div class="resource-list">

      <article class="resource">
        <h3>حفظ حریم خصوصی</h3>
        <p>
          هیچ‌کس نباید اطلاعات شخصی و روایت خصوصی
          افراد آسیب‌دیده را بدون رضایت آن‌ها منتشر کند.
        </p>
      </article>

      <article class="resource">
        <h3>حق دریافت حمایت</h3>
        <p>
          افراد آسیب‌دیده می‌توانند برای شناخت
          گزینه‌های حمایتی و حقوقی خود کمک بگیرند.
        </p>
      </article>

      <article class="resource">
        <h3>رسیدگی قانونی</h3>
        <p>
          بررسی اتهامات و تعیین مسئولیت کیفری باید
          از مسیر قانونی و با رعایت حقوق همه افراد انجام شود.
        </p>
      </article>

      <article class="resource">
        <h3>امنیت و احترام</h3>
        <p>
          قربانیان نباید به دلیل تجربه آسیب،
          مورد سرزنش یا تبعیض قرار بگیرند.
        </p>
      </article>

    </div>

  </div>
</section>

<!-- STORIES -->

<section id="stories">
  <div class="container">

    <div class="section-heading">
      <small>VOICES MATTER</small>
      <h2>داستان‌های شنیده‌نشده</h2>
      <p>
        هر تجربه انسانی شایسته احترام است.
      </p>
    </div>

    <div class="story-note">
      <h3>اینجا برای شنیدن است، نه قضاوت کردن.</h3>

      <p>
        در نسخه‌های آینده این بخش می‌تواند میزبان
        روایت‌های آگاهی‌بخش و ناشناس باشد؛
        تنها با رضایت آگاهانه صاحبان روایت،
        حذف اطلاعات هویتی و نظارت یک تیم مسئول.
      </p>

      <p>
        در حال حاضر امکان ارسال یا انتشار روایت شخصی
        در این وب‌سایت فعال نیست.
      </p>
    </div>

  </div>
</section>

<!-- CONTACT -->

<section id="contact" class="about">
  <div class="container">

    <div class="section-heading">
      <small>CONTACT</small>
      <h2>ارتباط با پروژه</h2>
      <p>
        این پروژه در مرحله آغازین توسعه قرار دارد.
        اطلاعات تماس رسمی پس از ایجاد سازوکار امن و
        مشخص شدن مسئولان پروژه منتشر خواهد شد.
      </p>
    </div>

    <div class="story-note">
      <h3>یک یادآوری مهم</h3>
      <p>
        این وب‌سایت در حال حاضر مرکز اورژانس،
        مرجع قضایی یا مرکز دریافت گزارش جرم نیست.
        اگر در خطر فوری هستی، به خدمات اضطراری
        محل زندگی‌ات یا یک فرد بزرگسال قابل اعتماد مراجعه کن.
      </p>
      <p>
        از ارسال نام، نشانی، شماره تماس یا اطلاعات
        خصوصی خودت و دیگران در بخش‌های عمومی اینترنت خودداری کن.
      </p>
    </div>

  </div>
</section>

</main>

<!-- FOOTER -->

<footer>
  <div class="container">

    <div class="footer-grid">

      <div>
        <h3>VOICELESS NO MORE</h3>
        <p>
          صدای بی‌صداها؛ برای حمایت، آگاهی
          و مطالبه عدالت.
        </p>
      </div>

      <div>
        <h3>دسترسی سریع</h3>
        <a href="#about">درباره ما</a>
        <a href="#mission">مأموریت ما</a>
        <a href="#support">حمایت از قربانیان</a>
      </div>

      <div>
        <h3>بخش‌های سایت</h3>
        <a href="#rights">حقوق و آگاهی</a>
        <a href="#stories">داستان‌ها</a>
        <a href="#contact">ارتباط با ما</a>
      </div>

    </div>

    <div class="copyright">
      © 2026 VOICELESS NO MORE — All Rights Reserved
      <br>
      این پروژه مستقل و در مرحله توسعه است.
    </div>

  </div>
</footer>

<script>
const menuBtn = document.getElementById('menuBtn');
const navLinks = document.getElementById('navLinks');

menuBtn.addEventListener('click', () => {
  const opened = navLinks.classList.toggle('open');
  menuBtn.setAttribute('aria-expanded', opened);
  menuBtn.textContent = opened ? '✕' : '☰';
});

document.querySelectorAll('.nav-links a').forEach(link => {
  link.addEventListener('click', () => {
    navLinks.classList.remove('open');
    menuBtn.setAttribute('aria-expanded', 'false');
    menuBtn.textContent = '☰';
  });
});
</script>

<!-- VOICELESS NO MORE - Contact Section -->
<style>
.contact-section {
  direction: rtl;
  padding: 65px 20px;
  background: #101722;
  color: #eee9df;
  font-family: Vazirmatn, sans-serif;
}
.contact-container {
  max-width: 680px;
  margin: auto;
  background: #182331;
  border: 1px solid #354354;
  border-radius: 18px;
  padding: 30px;
  box-shadow: 0 15px 40px #0005;
}
.contact-heading {
  text-align: center;
  margin-bottom: 28px;
}
.contact-heading h2 {
  color: #d7c5a3;
  font-size: 27px;
}
.contact-heading p {
  color: #b6c0cb;
  line-height: 2;
}
.contact-form label {
  display: block;
  margin: 18px 0 8px;
  color: #d7c5a3;
}
.contact-form input,
.contact-form textarea {
  width: 100%;
  box-sizing: border-box;
  padding: 13px;
  border-radius: 9px;
  border: 1px solid #455568;
  background: #101722;
  color: white;
  font: inherit;
  outline: none;
}
.contact-form input:focus,
.contact-form textarea:focus {
  border-color: #c9ae80;
}
.contact-form textarea {
  min-height: 145px;
  resize: vertical;
}
.contact-form button {
  width: 100%;
  margin-top: 24px;
  padding: 14px;
  border: none;
  border-radius: 9px;
  background: #c9ae80;
  color: #17202c;
  font: inherit;
  font-weight: bold;
  cursor: pointer;
}
.contact-form button:hover {
  background: #dfcba8;
}
.contact-note {
  color: #aab5c1;
  font-size: 12px;
  line-height: 2;
  margin-top: 18px;
}
</style>

<section class="contact-section" id="contact">
  <div class="contact-container">
    <div class="contact-heading">
      <h2>صدای تو شنیده می‌شود</h2>
      <p>
        اگر تجربه‌ای برای بیان کردن، پرسشی یا حرفی برای گفتن داری،
        می‌توانی از این طریق با تیم VOICELESS NO MORE ارتباط بگیری.
      </p>
    </div>

    <form class="contact-form"
          action="YOUR_FORMSPREE_ENDPOINT"
          method="POST">

      <label for="fullname">نام و نام خانوادگی</label>
      <input id="fullname" name="name"
             type="text" required maxlength="100"
             autocomplete="name"
             placeholder="نام کامل شما">

      <label for="email">آدرس ایمیل</label>
      <input id="email" name="email"
             type="email" required maxlength="150"
             autocomplete="email"
             placeholder="example@email.com">

      <label for="subject">موضوع پیام</label>
      <input id="subject" name="subject"
             type="text" required maxlength="150"
             placeholder="موضوع پیام شما">

      <label for="message">پیام شما</label>
      <textarea id="message" name="message"
                required maxlength="3000"
                placeholder="حرف‌هایت را اینجا بنویس..."></textarea>

      <button type="submit">ارسال پیام</button>

      <p class="contact-note">
        اطلاعات واردشده برای دریافت و پاسخ‌گویی به پیام استفاده می‌شود
        و در سایت به‌صورت عمومی نمایش داده نخواهد شد.
        لطفاً اطلاعات بسیار حساس، مدارک هویتی یا اطلاعات اشخاص دیگر را ارسال نکنید.
        این پروژه خدمات اورژانسی یا مشاوره تخصصی ارائه نمی‌دهد.
      </p>
    </form>
  </div>
</section>

</body>
</html>
