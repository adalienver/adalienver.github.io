---
layout: none
---
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Enver Adalı — Çeviribilim, Çeviri Teknolojileri & İngilizce Özel Ders</title>
  <meta name="description" content="Çeviribilim, Mütercim Tercümanlık perspektifi, yapay zekâ çağında çevirinin etik değeri, Subtitle Edit & SDL Trados Studio sunumları ve yüz yüze / online İngilizce özel ders.">
  <meta name="keywords" content="Enver Adalı, Çeviribilim, Mütercim Tercümanlık, Subtitle Edit sunumu, SDL Trados Studio eğitimi, yapay zeka ve çeviri, yüz yüze İngilizce özel ders, online İngilizce özel ders, YDS, YÖKDİL, TOEFL">
  <meta name="robots" content="index, follow">
  <link rel="canonical" href="https://adalienver.site/">

  <!-- Open Graph / Sosyal Medya Önizleme -->
  <meta property="og:type" content="website">
  <meta property="og:title" content="Enver Adalı — Çeviribilim, Çeviri Teknolojileri & Dil Eğitimi">
  <meta property="og:description" content="Mütercim Tercümanlık ve Çeviribilim perspektifi, Subtitle Edit & SDL Trados Studio atölyeleri ve yüz yüze / online İngilizce özel ders.">
  <meta property="og:url" content="https://adalienver.site/">

  <!-- FONTS -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,600;0,700;1,400&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --primary: #1a2b3d;
      --secondary: #2d5a6e;
      --accent: #d4a574;
      --muted: #5a6c7d;
      --light: #f5f7fa;
      --border: #dde3e8;
      --success: #2a7f62;
      --text: #1f2937;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html, body {
      height: 100%;
      overflow-x: hidden;
      width: 100%;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ffffff 0%, var(--light) 100%);
      color: var(--text);
      line-height: 1.65;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    /* NAVBAR */
    nav {
      background: white;
      border-bottom: 1px solid var(--border);
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-container {
      max-width: 980px;
      margin: 0 auto;
      padding: 0 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 70px;
      position: relative;
    }

    .nav-brand {
      font-family: 'Lora', serif;
      font-size: 1.3rem;
      font-weight: 700;
      color: var(--primary);
      text-decoration: none;
      letter-spacing: -0.5px;
    }

    .nav-brand small {
      display: block;
      font-size: 0.65rem;
      font-weight: 400;
      color: var(--accent);
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .nav-menu {
      display: flex;
      list-style: none;
      gap: 1.35rem;
      align-items: center;
    }

    .nav-menu a {
      text-decoration: none;
      color: var(--text);
      font-size: 0.9rem;
      font-weight: 500;
      transition: color 0.3s ease;
      position: relative;
    }

    .nav-menu a:hover,
    .nav-menu a.active {
      color: var(--accent);
    }

    .nav-menu a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--accent);
      transition: width 0.3s ease;
    }

    .nav-menu a:hover::after,
    .nav-menu a.active::after {
      width: 100%;
    }

    .nav-login-btn {
      background: var(--primary);
      color: #ffffff !important;
      padding: 0.45rem 0.95rem;
      border-radius: 5px;
      font-size: 0.85rem !important;
      transition: background 0.25s ease !important;
    }

    .nav-login-btn:hover {
      background: var(--secondary);
    }

    .nav-login-btn::after {
      display: none !important;
    }

    .hamburger {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
      padding: 10px;
      margin-right: -10px;
      z-index: 1001;
      position: relative;
      user-select: none;
      -webkit-tap-highlight-color: transparent;
    }

    .hamburger span {
      width: 24px;
      height: 2px;
      background: var(--primary);
      border-radius: 2px;
      transition: all 0.3s ease;
      display: block;
    }

    /* LAYOUT */
    .container {
      max-width: 900px;
      width: 100%;
      margin: 0 auto;
      padding: 3rem 2rem;
      flex: 1;
    }

    /* HERO */
    header {
      text-align: center;
      margin-bottom: 3.5rem;
      padding-bottom: 2rem;
    }

    h1 {
      font-family: 'Lora', serif;
      font-size: 2.35rem;
      font-weight: 700;
      color: var(--primary);
      letter-spacing: -0.5px;
      margin-bottom: 0.5rem;
    }

    .tagline {
      font-family: 'Lora', serif;
      font-size: 1.12rem;
      font-weight: 400;
      color: var(--secondary);
      font-style: italic;
      margin-bottom: 1.1rem;
    }

    .credentials {
      font-size: 0.92rem;
      color: var(--muted);
      margin-bottom: 1.5rem;
      letter-spacing: 0.2px;
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 1rem;
      flex-wrap: wrap;
      margin-top: 1.5rem;
    }

    .social-links a {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.65rem 1.25rem;
      background: var(--primary);
      color: #fff;
      text-decoration: none;
      border-radius: 4px;
      font-size: 0.9rem;
      font-weight: 500;
      transition: all 0.3s ease;
      border: 1px solid var(--primary);
    }

    .social-links a:hover {
      background: transparent;
      color: var(--primary);
      transform: translateY(-2px);
    }

    .social-links a.secondary {
      background: transparent;
      color: var(--primary);
      border: 1px solid var(--border);
    }

    .social-links a.secondary:hover {
      background: var(--primary);
      color: #fff;
    }

    .social-links a.accent-link {
      background: var(--accent);
      border-color: var(--accent);
      color: #fff;
    }

    .social-links a.accent-link:hover {
      background: var(--primary);
      border-color: var(--primary);
      color: #fff;
    }

    /* SECTIONS & CARDS */
    .section {
      background: #fff;
      border-radius: 8px;
      padding: 2.5rem;
      margin-bottom: 2.5rem;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
      border-top: 3px solid var(--primary);
      transition: box-shadow 0.3s ease;
    }

    .section:hover {
      box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
    }

    .section.accent {
      border-top-color: var(--accent);
    }

    .section.success {
      border-top-color: var(--success);
    }

    .section-label {
      display: inline-block;
      font-size: 0.75rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1px;
      color: var(--accent);
      margin-bottom: 0.8rem;
    }

    .section-label.success {
      color: var(--success);
    }

    h2 {
      font-family: 'Lora', serif;
      font-size: 1.7rem;
      font-weight: 600;
      color: var(--primary);
      margin-bottom: 1.2rem;
      line-height: 1.3;
    }

    h3 {
      font-family: 'Lora', serif;
      font-size: 1.2rem;
      font-weight: 600;
      color: var(--primary);
      margin-bottom: 0.8rem;
    }

    .section p {
      margin-bottom: 1rem;
    }

    .section p:last-child {
      margin-bottom: 0;
    }

    .quote {
      background: var(--light);
      border-left: 4px solid var(--accent);
      padding: 1.5rem;
      margin: 1.5rem 0;
      font-size: 1rem;
      font-style: italic;
      color: var(--primary);
      line-height: 1.8;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
      margin-top: 1.5rem;
    }

    .feature-box {
      background: var(--light);
      padding: 1.5rem;
      border-radius: 6px;
      border-left: 3px solid var(--accent);
      transition: all 0.3s ease;
    }

    .feature-box:hover {
      transform: translateY(-4px);
      border-left-color: var(--primary);
    }

    .feature-box strong {
      display: block;
      color: var(--primary);
      font-size: 1rem;
      margin-bottom: 0.6rem;
    }

    .feature-box p {
      font-size: 0.9rem;
      color: var(--muted);
      line-height: 1.6;
      margin: 0;
    }

    .cta-group {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      align-items: center;
      margin-top: 1.8rem;
      padding-top: 1.5rem;
      border-top: 1px solid var(--border);
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.7rem 1.5rem;
      border-radius: 4px;
      font-size: 0.92rem;
      font-weight: 600;
      text-decoration: none;
      transition: all 0.3s ease;
      cursor: pointer;
      border: none;
    }

    .btn-primary {
      background: var(--primary);
      color: #fff;
      border: 1px solid var(--primary);
    }

    .btn-primary:hover {
      background: transparent;
      color: var(--primary);
      transform: translateY(-2px);
    }

    .btn-secondary {
      background: var(--accent);
      color: #fff;
      border: 1px solid var(--accent);
    }

    .btn-secondary:hover {
      background: var(--primary);
      border-color: var(--primary);
      transform: translateY(-2px);
    }

    .btn-outline {
      background: transparent;
      color: var(--primary);
      border: 1px solid var(--border);
    }

    .btn-outline:hover {
      background: var(--light);
      border-color: var(--primary);
    }

    .btn-success {
      background: var(--success);
      color: #fff;
      border: 1px solid var(--success);
    }

    .btn-success:hover {
      background: transparent;
      color: var(--success);
      transform: translateY(-2px);
    }

    .badge {
      display: inline-block;
      background: #ecf5e8;
      color: var(--success);
      padding: 0.35rem 0.85rem;
      border-radius: 999px;
      font-size: 0.8rem;
      font-weight: 600;
      border: 1px solid #c7e5b4;
    }

    .portal-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.5rem;
      margin-top: 1.5rem;
    }

    .portal-card {
      display: block;
      padding: 1.5rem;
      border: 1px solid var(--border);
      border-radius: 6px;
      text-decoration: none;
      color: inherit;
      transition: all 0.3s ease;
      background: #fafbfc;
    }

    .portal-card:hover {
      border-color: var(--accent);
      background: var(--light);
      transform: translateY(-4px);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    }

    .portal-card strong {
      display: block;
      font-size: 1.05rem;
      color: var(--primary);
      margin-bottom: 0.4rem;
    }

    .portal-card .description {
      font-size: 0.85rem;
      color: var(--muted);
      margin-bottom: 0.8rem;
    }

    .portal-card .portal-tag {
      display: inline-block;
      font-size: 0.75rem;
      color: var(--accent);
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    /* FOOTER */
    footer {
      background: var(--primary);
      color: white;
      padding: 3.5rem 2rem 2.5rem;
      margin-top: auto;
    }

    .footer-container {
      max-width: 900px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 2rem;
      margin-bottom: 2rem;
    }

    .footer-section h4 {
      font-family: 'Lora', serif;
      font-size: 1.05rem;
      margin-bottom: 1rem;
      color: var(--accent);
    }

    .footer-section ul {
      list-style: none;
    }

    .footer-section ul li {
      margin-bottom: 0.7rem;
    }

    .footer-section a {
      color: #e2e8f0;
      text-decoration: none;
      font-size: 0.9rem;
      transition: color 0.3s ease;
    }

    .footer-section a:hover {
      color: var(--accent);
    }

    .footer-contact {
      font-size: 0.9rem;
      line-height: 1.8;
    }

    .footer-contact strong {
      display: block;
      color: var(--accent);
      margin-bottom: 0.2rem;
    }

    .footer-divider {
      border-top: 1px solid rgba(255, 255, 255, 0.12);
      padding-top: 2rem;
      text-align: center;
      color: #94a3b8;
      font-size: 0.85rem;
    }

    /* RESPONSIVE */
    @media (max-width: 860px) {
      .nav-container {
        padding: 0 1.2rem;
      }

      .nav-menu {
        display: none;
        position: absolute;
        top: 70px;
        left: 0;
        right: 0;
        flex-direction: column;
        background: white;
        padding: 1.5rem;
        border-bottom: 1px solid var(--border);
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.12);
        z-index: 1000;
        gap: 1rem;
      }

      .nav-menu.active {
        display: flex;
      }

      .hamburger {
        display: flex;
      }

      .container {
        padding: 1.5rem 1.2rem;
      }

      .features-grid,
      .portal-grid {
        grid-template-columns: 1fr;
      }

      h1 {
        font-size: 1.85rem;
      }

      h2 {
        font-size: 1.4rem;
      }

      .section {
        padding: 1.5rem;
      }

      .social-links {
        gap: 0.8rem;
      }

      .social-links a {
        padding: 0.5rem 1rem;
        font-size: 0.85rem;
      }

      .footer-container {
        grid-template-columns: 1fr;
        gap: 1.5rem;
      }
    }
  </style>
</head>
<body>

  <!-- NAVBAR -->
  <nav>
    <div class="nav-container">
      <a href="/" class="nav-brand">
        <small>Enver Adalı</small>
        Çeviribilim & Dil
      </a>
      <ul class="nav-menu">
        <li><a href="/" class="active" aria-current="page">Ana Sayfa</a></li>
        <li><a href="/edebiyat/">Edebî Seçki</a></li>
        <li><a href="/kaynaklar/">Kaynaklar</a></li>
        <li><a href="/podcast.html">Podcast</a></li>
        <li><a href="#iletisim">İletişim</a></li>
        <li><a href="/login.html" class="nav-login-btn">Öğrenci Girişi</a></li>
      </ul>
      <div class="hamburger" role="button" aria-label="Menüyü Aç/Kapat" tabindex="0">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </nav>

  <!-- MAIN CONTENT -->
  <div class="container">

    <!-- HERO -->
    <header id="ana-sayfa">
      <h1>Enver Adalı</h1>
      <p class="tagline">Çeviribilim • Çeviri Teknolojileri • İngiliz Dili Eğitimi</p>
      <div class="credentials">
        <span>İngilizce Mütercim Tercümanlık (Lisans) & İngiliz Dili ve Edebiyatı (Yüksek Lisans)</span>
      </div>
      <div class="social-links">
        <a href="/kaynaklar/#name" class="accent-link">
          ✉ Yüz Yüze & Online İletişim
        </a>
        <a href="mailto:enveradali195@gmail.com" class="secondary">
          enveradali195@gmail.com
        </a>
        <a href="https://www.linkedin.com/in/enver-adalı/" target="_blank" rel="noopener noreferrer">
          💼 LinkedIn
        </a>
      </div>
    </header>

    <!-- ÇEVİRİBİLİM, MÜTERCİM TERCÜMANLIK & YAPAY ZEKÂ PERSPEKTİFİ -->
    <section class="section" id="ceviribilim-perspektif">
      <span class="section-label">Disiplinler Arası Bakış & Mesleki Savunu</span>
      <h2>Yapay Zekâ Çağında Mütercim Tercümanlık ve Çeviribilim Neden Daha Kritik?</h2>
      <p>Büyük Dil Modelleri ve makine çevirisi araçları teknik hız kazandırmış olsa da, <strong>yapay zekâ çevirmenliği bitirmemiş; aksine nitelikli insan uzmanlığına duyulan ihtiyacı derinleştirmiştir.</strong> Çeviri, kelimeleri istatistiksel olasılıklarla yan yana dizmek değil; metnin tarihsel arka planını, ideolojik katmanlarını, kültürel göndermelerini ve bağlamsal ağırlığını yeniden inşa etme eylemidir.</p>
      <p>Bu nedenle <strong>Mütercim Tercümanlık ve Çeviribilim bölümleri</strong>, yalnızca yabancı dil bilen bireyler değil; teknolojiyi eleştirel akılla yöneten, metne müdahale sınırını bilen ve kültürler arası iletişimin sorumluluğunu üstlenen uzmanlar yetiştirdiği için her zamankinden daha fazla önem kazanmaktadır.</p>

      <div class="quote">
        "Yapay zekâ olası olanı üretir; çevirmen ise metnin <em>etik sorumluluğunu</em>, <em>kültürel sadakatini</em> ve <em>insani anlamını</em> kurar."
      </div>

      <div class="features-grid">
        <div class="feature-box">
          <strong>⚖️ Etik Sorumluluk & Güven</strong>
          <p>Hukuki, tıbbi, akademik ve edebî metinlerde makine halüsinasyonlarını ve anlam kaymalarını denetleyecek etik özne yalnızca çevirmendir.</p>
        </div>
        <div class="feature-box">
          <strong>🧠 Kültürel & Yorumbilimsel Derinlik</strong>
          <p>İroni, alt metin, yerel deyimler ve tarihsel hafıza algoritmik kalıplara sığmaz; yorumlayıcı insan bilinci gerektirir.</p>
        </div>
        <div class="feature-box">
          <strong>⚙️ Teknolojiyi Yöneten Çevirmen</strong>
          <p>Çeviribilim eğitimi, çevirmeni teknolojinin pasif izleyicisi değil; CAT ve altyazı yazılımlarına hükmeden profesyonel aktör kılar.</p>
        </div>
      </div>
    </section>

    <!-- SUBTITLE EDIT & SDL TRADOS STUDIO SUNUMLARI -->
    <section class="section success" id="ceviribilim-atolye">
      <span class="section-label success">Uygulamalı Sunumlar & Mesleki Dayanışma</span>
      <h2>Subtitle Edit & SDL Trados Studio Sunumları</h2>
      <p>Mütercim Tercümanlık ve Çeviribilim öğrencilerinin sektör standartlarına hazırlıklı adım atmalarına katkı sunmak amacıyla; uygulamalı <strong>Subtitle Edit</strong> ve <strong>SDL Trados Studio</strong> sunumları ve atölye çalışmaları gerçekleştiriyorum.</p>
      
      <div class="quote">
        <strong>Subtitle Edit</strong> sunumlarında zaman kodlama (time-coding), okuma hızı (CPS) dengesi, sahne geçişi senkronizasyonu ve görsel-işitsel çevirinin etik ilkeleri; <strong>SDL Trados Studio</strong> oturumlarında ise çeviri belleği (Translation Memory), terim yönetimi ve kalite güvencesi iş akışları uygulamalı olarak ele alınır.
      </div>

      <div class="cta-group">
        <p style="flex: 1; color: var(--muted); font-size: 0.9rem;">Öğrenci toplulukları, bölüm etkinlikleri veya birebir yazılım danışmanlığı için yüz yüze ve online iletişime geçebilirsiniz.</p>
        <a href="/kaynaklar/#name" class="btn btn-success">
          🎬 Sunum & Atölye İletişimi
        </a>
      </div>
    </section>

    <!-- ÖZEL DERS (ÖZET & DENGELİ) -->
    <section class="section accent" id="dersler">
      <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 1rem; margin-bottom: 1rem;">
        <div>
          <span class="section-label">Birebir Dil Eğitimi</span>
          <h2>Yüz Yüze & Online İngilizce Özel Ders</h2>
        </div>
        <span class="badge">Yüz Yüze & Online</span>
      </div>

      <p>Akademik ve dilbilimsel altyapımla; öğrencinin hedefine ve mevcut seviyesine göre yapılandırılmış <strong>yüz yüze ve online İngilizce özel ders</strong> desteği de sunuyorum.</p>

      <div class="features-grid">
        <div class="feature-box">
          <strong>📚 Akademik Sınavlar (YDS, YÖKDİL, TOEFL)</strong>
          <p>Akademik okuma stratejileri, ileri sözcük bilgisi, bağlaç analizi ve çeviri odaklı sınav hazırlığı.</p>
        </div>
        <div class="feature-box">
          <strong>🎯 Okul Takviyesi & LGS İngilizce</strong>
          <p>Müfredata uyumlu kazanım pekiştirme, soru çözüm teknikleri ve temelden kalıcı dil becerisi.</p>
        </div>
        <div class="feature-box">
          <strong>🗣️ Konuşma & Telaffuz Pratiği</strong>
          <p>Akıcı sözlü ifade, fonetik telaffuz düzeltme ve akademik/günlük iletişim becerisi.</p>
        </div>
      </div>

      <div class="cta-group">
        <p style="flex: 1; color: var(--muted); font-size: 0.9rem;">Yüz yüze veya online ders planlaması ve ön görüşme için iletişim formunu kullanabilirsiniz.</p>
        <a href="/kaynaklar/#name" class="btn btn-secondary">
          ✉ Yüz Yüze & Online İletişim
        </a>
      </div>
    </section>

    <!-- KURUMSAL BAĞLANTILAR -->
    <section class="section">
      <h2>Akademik & Kurumsal Bağlantılar</h2>
      <div class="portal-grid">
        <a href="https://www.beykent.edu.tr/aday-ogrenci/bolumler-programlar/lisans/fen-edebiyat-fakultesi/ingilizce-mutercim-ve-tercumanlik" target="_blank" rel="noopener noreferrer" class="portal-card">
          <strong>İngilizce Mütercim ve Tercümanlık</strong>
          <div class="description">İstanbul Beykent Üniversitesi • Lisans Programı</div>
          <span class="portal-tag">Bölüm Detayı →</span>
        </a>
        <a href="https://lisansustu.beykent.edu.tr/yuksek-lisans/ingiliz-dili-ve-edebiyati-abd" target="_blank" rel="noopener noreferrer" class="portal-card">
          <strong>İngiliz Dili ve Edebiyatı</strong>
          <div class="description">Lisansüstü Eğitim Enstitüsü</div>
          <span class="portal-tag">Enstitü Portalı →</span>
        </a>
      </div>
    </section>

    <!-- KAYNAKLAR MERKEZİ -->
    <section class="section" style="text-align: center; background: linear-gradient(135deg, var(--light) 0%, #fff 100%);">
      <h3 style="margin-top: 0;">📚 Kaynaklar Merkezi & İletişim Formu</h3>
      <p style="color: var(--muted); margin-bottom: 1.5rem;">Derlem (korpus) veri tabanları, collocation sözlükleri, dinleme platformları, dikte alıştırmaları ve doğrudan yüz yüze / online iletişim formu.</p>
      <a href="/kaynaklar/" class="btn btn-outline">
        Kaynaklara & İletişim Formuna Git →
      </a>
    </section>

  </div>

  <!-- FOOTER -->
  <footer id="iletisim">
    <div class="footer-container">
      <div class="footer-section">
        <h4>Yüz Yüze & Online İletişim</h4>
        <div class="footer-contact">
          <strong>E-posta:</strong>
          <a href="mailto:enveradali195@gmail.com">enveradali195@gmail.com</a>
          <br><br>
          <strong>İletişim Formu:</strong>
          <a href="/kaynaklar/#name">Yüz Yüze & Online İletişim Formu →</a>
          <br><br>
          <strong>Profesyonel Ağ:</strong>
          <a href="https://www.linkedin.com/in/enver-adalı/" target="_blank" rel="noopener noreferrer">LinkedIn Profili</a>
        </div>
      </div>

      <div class="footer-section">
        <h4>Sayfalar</h4>
        <ul>
          <li><a href="/">Ana Sayfa</a></li>
          <li><a href="/edebiyat/">Edebî Seçki</a></li>
          <li><a href="/kaynaklar/">Kaynaklar & İletişim Formu</a></li>
          <li><a href="/podcast.html">Podcast</a></li>
          <li><a href="/login.html">Öğrenci Girişi</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h4>Çalışma & Uzmanlık Alanları</h4>
        <ul>
          <li><a href="#ceviribilim-perspektif">Çeviribilim & Çeviri Etiği</a></li>
          <li><a href="#ceviribilim-atolye">Subtitle Edit Uygulamalı Sunumu</a></li>
          <li><a href="#ceviribilim-atolye">SDL Trados Studio Atölyesi</a></li>
          <li><a href="#dersler">Yüz Yüze & Online İngilizce Özel Ders</a></li>
        </ul>
      </div>
    </div>

    <div class="footer-divider">
      <p>© 2026 Enver Adalı. Tüm hakları saklıdır.</p>
      <p style="margin-top: 0.4rem;">Çeviribilim • Mütercim Tercümanlık • İngiliz Dili Eğitimi</p>
    </div>
  </footer>

  <!-- MOBİL MENÜ TETİKLEYİCİ -->
  <script>
    document.addEventListener('DOMContentLoaded', function () {
      const hamburger = document.querySelector('.hamburger');
      const navMenu = document.querySelector('.nav-menu');

      if (hamburger && navMenu) {
        hamburger.addEventListener('click', function (e) {
          e.stopPropagation();
          navMenu.classList.toggle('active');
        });

        document.querySelectorAll('.nav-menu a').forEach(function (link) {
          link.addEventListener('click', function () {
            navMenu.classList.remove('active');
          });
        });

        document.addEventListener('click', function (e) {
          if (!navMenu.contains(e.target) && !hamburger.contains(e.target)) {
            navMenu.classList.remove('active');
          }
        });
      }
    });
  </script>

  <!-- ARKA PLAN YAPISAL VERİ SCHEMA.ORG (JSON-LD) -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@graph": [
      {
        "@type": "Person",
        "@id": "https://adalienver.site/#person",
        "name": "Enver Adalı",
        "url": "https://adalienver.site/",
        "email": "enveradali195@gmail.com",
        "jobTitle": "Çeviribilimci, Mütercim Tercüman & İngilizce Eğitmeni",
        "description": "Çeviribilim, çeviri etiği, Subtitle Edit ve SDL Trados Studio uygulamalı sunumları ile yüz yüze ve online İngilizce özel ders.",
        "knowsAbout": [
          "Çeviribilim",
          "Mütercim Tercümanlık",
          "Çeviri Etiği",
          "Subtitle Edit",
          "SDL Trados Studio",
          "İngiliz Dili Eğitimi"
        ],
        "sameAs": [
          "https://www.linkedin.com/in/enver-adalı/"
        ]
      },
      {
        "@type": "ItemList",
        "name": "Sunum, Atölye ve Eğitim Alanları",
        "itemListElement": [
          {
            "@type": "Course",
            "position": 1,
            "name": "Subtitle Edit Uygulamalı Altyazı Çevirisi Sunumu",
            "description": "Mütercim Tercümanlık ve Çeviribilim öğrencilerine yönelik zaman kodlama, senkronizasyon ve altyazı çevirisi etiği sunumu.",
            "provider": { "@id": "https://adalienver.site/#person" }
          },
          {
            "@type": "Course",
            "position": 2,
            "name": "SDL Trados Studio Uygulamalı Eğitimi",
            "description": "Çeviri belleği, terim yönetimi ve kalite kontrol süreçleri üzerine uygulamalı eğitim.",
            "provider": { "@id": "https://adalienver.site/#person" }
          },
          {
            "@type": "Course",
            "position": 3,
            "name": "Yüz Yüze & Online İngilizce Özel Ders",
            "description": "YDS, YÖKDİL, TOEFL, LGS ve konuşma pratiğine yönelik birebir İngilizce eğitimi.",
            "provider": { "@id": "https://adalienver.site/#person" }
          }
        ]
      }
    ]
  }
  </script>

</body>
</html>
