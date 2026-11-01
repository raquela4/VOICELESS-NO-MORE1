
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#101722">

<title>VOICELESS NO MORE</title>

<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  background: #101722;
  color: #eee9df;
  font-family: Vazirmatn, sans-serif;
  line-height: 1.9;
}

a {
  color: inherit;
  text-decoration: none;
}

header {
  position: sticky;
  top: 0;
  z-index: 10;
  background: rgba(13, 20, 30, .96);
  border-bottom: 1px solid #293647;
  padding: 14px 7%;
}

.nav {
  max-width: 1150px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 15px;
}

.logo {
  color: #d7c5a3;
  font-size: 19px;
  font-weight: 800;
  letter-spacing: 1px;
}

.nav-links {
  display: flex;
  gap: 22px;
  font-size: 13px;
  color: #c4ccd5;
}

.nav-links a:hover {
  color: #d7c5a3;
}

.hero {
  min-height: 590px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 20px;
  background:
    linear-gradient(rgba(8,14,23,.80), rgba(8,14,23,.96)),
    url("https://images.unsplash.com/photo-1519608487953-e999c86e7455?auto=format&fit=crop&w=1600&q=85")
    center/cover;
}

.hero-content {
  max-width: 800px;
}

.hero h1 {
  color: #d7c5a3;
  font-size: clamp(34px, 7vw, 66px);
  line-height: 1.4;
  letter-spacing: 2px;
}

.hero h2 {
  font-size: 21px;
  font-weight: 500;
  margin: 18px 0;
}

.hero p {
  color: #c2c9d2;
  max-width: 650px;
  margin: auto;
}

.main-button {
  display: inline-block;
  margin-top: 30px;
  padding: 11px 28px;
  border-radius: 8px;
  background: #c9ae80;
  color: #17202c;
  font-weight: 700;
}

section {
  padding: 75px 20px;
}

.container {
  max-width: 1050px;
  margin: auto;
}

.section-title {
  color: #d7c5a3;
  font-size: 29px;
  text-align: center;
  margin-bottom: 20px;
}

.section-description {
  color: #b9c2cd;
  text-align: center;
  max-width: 750px;
  margin: auto;
}

.about {
  background: #151f2d;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  margin-top: 35px;
}

.card {
  background: #1b2939;
  border: 1px solid #344457;
  border-radius: 13px;
  padding: 25px;
  text-align: center;
}

.card h3 {
  color: #d7c5a3;
  margin-bottom: 10px;
}

.card p {
  color: #b9c2cd;
  font-size: 14px;
}

.mission-list {
  max-width: 750px;
  margin: 30px auto 0;
}

.mission-list div {
  padding: 15px;
  margin: 12px 0;
  background: #1b2939;
  border-right: 3px solid #c9ae80;
  border-radius: 7px;
}

.contact-section {
  background: #151f2d;
}

.contact-container {
  max-width: 680px;
  margin: 30px auto 0;
  background: #1b2939;
  border: 1px solid #35465a;
  border-radius: 18px;
  padding: 30px;
  box-shadow: 0 15px 40px #0005;
}

.contact-heading {
  text-align: center;
  margin-bottom: 25px;
}

.contact-heading h3 {
  color: #d7c5a3;
  font-size: 23px;
}

.contact-heading p {
  color: #b9c2cd;
  font-size: 14px;
}

.contact-form label {
  display: block;
  margin: 17px 0 7px;
  color: #d7c5a3;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 13px;
  border-radius: 9px;
  border: 1px solid #455568;
  background: #101722;
  color: white;
  font-family: inherit;
  font-size: 14px;
  outline: none;
}

.contact-form input:focus,
.contact-form textarea:focus {
  border-color: #c9ae80;
}

.contact-form textarea {
  min-height: 140px;
  resize: vertical;
}

.contact-form button {
  width: 100%;
  margin-top: 23px;
  padding: 13px;
  border: none;
  border-radius: 9px;
  background: #c9ae80;
  color: #17202c;
  font-family: inherit;
  font-size: 16px;
  font-weight: 700;
  cursor: pointer;
}

.contact-form button:hover {
  background: #dfcba8;
}

.privacy {
  color: #aab5c1;
  font-size: 12px;
  line-height: 2.2;
  margin-top: 17px;
}

.consent {
  display: flex !important;
  align-items: flex-start;
  gap: 9px;
  color: #b9c2cd !important;
  font-size: 12px;
}

.consent input {
  width: auto;
  margin-top: 7px;
}

footer {
  padding: 30px 20px;
  background: #0b111a;
  text-align: center;
  color: #8995a4;
  font-size: 13px;
}

footer strong {
  color: #d7c5a3;
}

@media(max-width: 650px) {
  .nav {
    flex-direction: column;
  }

  .nav-links {
    flex-wrap: wrap;
    justify-content: center;
    gap: 12px;
    font-size: 12px;
  }

  .hero {
    min-height: 500px;
  }

  .contact-container {
    padding: 20px;
  }
}
</style>
</head>

<body>

<header>
  <nav class="nav">
    <div class="logo">VOICELESS NO MORE</div>

    <div class="nav-links">
      <a href="#home">خانه</a>
      <a href="#about">درباره ما</a>
      <a href="#mission">اهداف</a>
      <a href="#contact">ارتباط با ما</a>
    </div>
  </nav>
</header>

<main>

<section class="hero" id="home">
  <div class="hero-content">
    <h1>VOICELESS NO MORE</h1>

    <h2>صدایی برای کسانی که شنیده نشدند</h2>

    <p>
      ما باور داریم هیچ انسانی نباید در برابر بی‌عدالتی،
      آسیب و نادیده گرفته شدن تنها بماند.
      آگاهی، حمایت و مسئولیت‌پذیری اجتماعی
      نقطه شروع تغییر هستند.
    </p>

    <a href="#about" class="main-button">
      بیشتر درباره ما بدانید
    </a>
  </div>
</section>

<section class="about" id="about">
  <div class="container">
    <h2 class="section-title">درباره ما</h2>

    <p class="section-description">
      VOICELESS NO MORE یک پروژه مستقل آگاهی‌بخشی
      با تمرکز بر حمایت از قربانیان و افزایش آگاهی
      درباره حقوق انسانی در ایران است.
      هدف ما ایجاد فضایی برای شنیده شدن صداها،
      شناخت حقوق و ترویج مسئولیت اجتماعی است.
    </p>

    <div class="cards">
      <div class="card">
        <h3>حمایت</h3>
        <p>
          فراهم کردن اطلاعات و راهنمایی برای شناخت
          مسیرهای امن دریافت کمک.
        </p>
      </div>

      <div class="card">
        <h3>آگاهی</h3>
        <p>
          افزایش آگاهی عمومی درباره حقوق انسانی
          و اهمیت شنیده شدن صدای افراد.
        </p>
      </div>

      <div class="card">
        <h3>عدالت</h3>
        <p>
          ترویج پاسخ‌گویی، مسئولیت‌پذیری
          و اهمیت پیگیری قانونی و منصفانه.
        </p>
      </div>
    </div>
  </div>
</section>

<section id="mission">
  <div class="container">
    <h2 class="section-title">مسیر و اهداف ما</h2>

    <p class="section-description">
      تغییر از آگاهی شروع می‌شود.
      ما تلاش می‌کنیم فضایی مسئولانه برای
      شناخت حقوق و حمایت اجتماعی ایجاد کنیم.
    </p>

    <div class="mission-list">
      <div>آموزش و انتشار اطلاعات عمومی درباره حقوق افراد</div>
      <div>معرفی مسیرهای معتبر دریافت کمک و مشاوره تخصصی</div>
      <div>ترویج احترام، همدلی و مسئولیت اجتماعی</div>
      <div>افزایش آگاهی درباره اهمیت عدالت و پاسخ‌گویی</div>
    </div>
  </div>
</section>

<section class="contact-section" id="contact">
  <div class="container">

    <h2 class="section-title">ارتباط با ما</h2>

    <p class="section-description">
      اگر پرسشی، پیشنهادی یا نظری درباره فعالیت‌های
      پروژه دارید، می‌توانید از طریق فرم زیر با ما
      ارتباط برقرار کنید.
    </p>

    <div class="contact-container">

      <div class="contact-heading">
        <h3>صدای تو شنیده می‌شود</h3>
        <p>پیامت را برای تیم پروژه ارسال کن.</p>
      </div>

      <form class="contact-form"
            action="https://formspree.io/f/xljjpqbb"
            method="POST">

        <label for="fullname">نام و نام خانوادگی</label>

        <input
          id="fullname"
          name="name"
          type="text"
          maxlength="100"
          autocomplete="name"
          placeholder="نام کامل شما"
          required
        >

        <label for="email">آدرس ایمیل</label>

        <input
          id="email"
          name="email"
          type="email"
          maxlength="150"
          autocomplete="email"
          placeholder="example@email.com"
          required
        >

        <label for="subject">موضوع پیام</label>

        <input
          id="subject"
          name="subject"
          type="text"
          maxlength="150"
          placeholder="موضوع پیام شما"
          required
        >

        <label for="message">متن پیام</label>

        <textarea
          id="message"
          name="message"
          maxlength="3000"
          placeholder="پیامت را اینجا بنویس..."
          required
        ></textarea>

        <label class="consent">
          <input type="checkbox" required>
          <span>
            می‌دانم اطلاعاتم برای دریافت و پاسخ‌گویی
            به پیام استفاده می‌شود و ممکن است توسط
            سرویس فرم پردازش شود.
          </span>
        </label>

        <button type="submit">
          ارسال پیام
        </button>

        <p class="privacy">
          اطلاعات شما در سایت به‌صورت عمومی نمایش داده نمی‌شود.
          با این حال، محرمانگی مطلق تضمین نمی‌شود؛
          سرویس Formspree ممکن است اطلاعات فنی را نیز پردازش کند.
          لطفاً اطلاعات بسیار حساس، مدارک هویتی،
          نشانی منزل یا اطلاعات خصوصی اشخاص دیگر را ارسال نکنید.
          این فرم برای ارتباط عمومی است و محل دریافت گزارش
          فوری، رسیدگی حقوقی یا مشاوره تخصصی نیست.
        </p>

      </form>
    </div>
  </div>
</section>

</main>

<footer>
  <strong>VOICELESS NO MORE</strong>

  <p>صدایی برای کسانی که شنیده نشدند.</p>

  <p>© 2026 VOICELESS NO MORE</p>
</footer>

</body>
</html>
