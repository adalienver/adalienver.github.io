---
layout: none
---

<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Online & Birebir İngilizce Özel Ders | YDS, TOEFL & Akademik Çeviri - Enver Adalı</title>
  <meta name="description" content="Birebir ve online İngilizce özel ders. YDS, YÖKDİL, TOEFL ve LGS sınav hazırlığı, akademik çeviri ve bireye özel çalışma programı.">
  <meta name="keywords" content="ingilizce özel ders, online ingilizce dersi, yds özel ders, toefl hazırlık, yökdil dersi, akademik çeviri">
  <link rel="canonical" href="https://adalienver.site/">

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
      max-width: 900px;
      margin: 0 auto;
      padding: 0 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 70px;
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
      gap: 2rem;
      align-items: center;
    }

    .nav-menu a {
      text-decoration: none;
      color: var(--text);
      font-size: 0.92rem;
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

    .hamburger {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
    }

    .hamburger span {
      width: 24px;
      height: 2px;
      background: var(--primary);
      border-radius: 2px;
      transition: all 0.3s ease;
    }

    /* LAYOUT */
    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 2rem;
      flex: 1;
    }

    /* HERO */
    header {
      text-align: center;
      margin-bottom: 4rem;
      padding-bottom: 2.5rem;
    }

    h1 {
      font-family: 'Lora', serif;
      font-size: 2.2rem;
      font-weight: 700;
      color: var(--primary);
      letter-spacing: -0.5px;
      margin-bottom: 0.5rem;
    }

    .tagline {
      font-family: 'Lora', serif;
      font-size: 1.1rem;
      font-weight: 400;
      color: var(--secondary);
      font-style: italic;
      margin-bottom: 1.2rem;
    }

    .credentials {
      font-size: 0.9rem;
      color: var(--muted);
      margin-bottom: 1.5rem;
      letter-spacing: 0.3px;
    }

    .credentials span {
      display: inline-block;
      margin: 0 0.5rem;
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 1.2rem;
      flex-wrap: wrap;
      margin-top: 1.5rem;
    }

    .social-links a {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.6rem 1.2rem;
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
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
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
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
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
    @media (max-width: 768px) {
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
        gap: 1rem;
      }

      .nav-menu.active {
        display: flex;
      }

      .hamburger {
        display: flex;
      }

      .container {
        padding: 2rem 1.5rem;
      }

      h1 {
        font-size: 1.8rem;
      }

      h2 {
        font-size: 1.4rem;
      }

      .section {
        padding: 1.8rem;
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
        <li><a href="#ana-sayfa" class="active">Ana Sayfa</a></li>
        <li><a href="#hakkinda">Perspektif</a></li>
        <li><a href="#dersler">Özel Ders</a></li>
        <li><a href="/kaynaklar/">Kaynaklar</a></li>
        <li><a href="#iletisim">İletişim</a></li>
      </ul>
      <div class="hamburger">
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
      <p class="tagline">Çeviribilim • Mütercim Tercümanlık • İngiliz Dili</p>
      <div class="credentials">
        <span>İstanbul Beykent Üniversitesi Mezunu</span>
      </div>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/enver-adalı-195" target="_blank" rel="noopener noreferrer">
          💼 LinkedIn Profili
        </a>
        <a href="mailto:enveradali195@gmail.com" class="secondary">
          ✉ enveradali195@gmail.com
        </a>
      </div>
    </header>

    <!-- HAKKINDA / PERSPEKTİF -->
    <section class="section" id="hakkinda">
      <span class="section-label">İçgörü & Perspektif</span>
      <h2>Çeviribilim Neden Hayatidir?</h2>
      <p>Büyük Dil Modelleri teknik hız kazandırmış olsa da, çeviri mekanik bir sözcük eşleme değildir. Metnin tarihsel katmanlarını, ideolojik nüanslarını ve edebi dokusunu anlamlandıracak <strong>insan bilinci</strong> her zamankından çok ihtiyaç duyuluyor.</p>
      
      <div class="quote">
        "Yapay zekâ istatistiksel olasılıklarla sözcük dizer; çevirmen ise metnin <em>ruhunu</em>, <em>etik sorumluluğunu</em> ve <em>estetik dengesini</em> kurar."
      </div>

      <div class="features-grid">
        <div class="feature-box">
          <strong>🧠 Yorumbilim & Kültür</strong>
          <p>Makineler kültürel hafızayı, örtük anlamları ve edebi ironiyi sezgisel olarak kavrayamaz.</p>
        </div>
        <div class="feature-box">
          <strong>⚙️ Teknoloji + İnsan</strong>
          <p>Geleceğin çevirmeni yapay zekânın rakibi değil; araçları eleştirel gözle yöneten entelektüel yöneticidir.</p>
        </div>
        <div class="feature-box">
          <strong>📚 Disiplinler Arası</strong>
          <p>Dilbilim, sosyoloji, tarih ve estetik bilgisinin sentezi çeviriyi önemli hâle getirir.</p>
        </div>
      </div>
    </section>

    <!-- ÖZEL DERS -->
    <section class="section accent" id="dersler">
      <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 1rem; margin-bottom: 1rem;">
        <div>
          <span class="section-label">Eğitim & Danışmanlık</span>
          <h2>İngilizce Özel Ders</h2>
        </div>
        <span class="badge">Kontenjan Açık</span>
      </div>

      <p>Ortaokul takviyesinden LGS hazırlığına, lise dil gelişiminden yetişkinlere ve akademik sınavlara (YDS, YÖKDİL, TOEFL) kadar kişiselleştirilmiş birebir ve online çalışma programları.</p>

      <div class="features-grid">
        <div class="feature-box">
          <strong>🎯 LGS & Okul Takviyesi</strong>
          <p>5–8. sınıf MEB müfredatına tam uyumlu kazanım pekiştirme ve yeni nesil soru çözümü.</p>
        </div>
        <div class="feature-box">
          <strong>📚 Akademik Sınavlar</strong>
          <p>YDS, YÖKDİL ve YDT hazırlığı. Akademik çeviri, sözcük dağarcığı ve strateji odaklı okuma.</p>
        </div>
        <div class="feature-box">
          <strong>🗣️ İletişim & Telaffuz</strong>
          <p>Akıcı konuşma pratiği, doğru fonetik telaffuz ve mesleki/akademik ifade becerisi.</p>
        </div>
      </div>

      <div class="cta-group">
        <p style="flex: 1; color: var(--muted); font-size: 0.9rem;">Ders programı ve seviye tespiti için doğrudan yazabilirsiniz.</p>
        <a href="mailto:enveradali195@gmail.com?subject=İngilizce%20Özel%20Ders%20Talebi" class="btn btn-secondary">
          ✉ Ders Talep Et
        </a>
      </div>
    </section>

    <!-- MESLEKİ DAYANIŞMA -->
    <section class="section success">
      <span class="section-label success">Ücretsiz Atölyeler</span>
      <h2>Mesleki Dayanışma</h2>
      <p>Çeviribilim disiplinine katkı sunmak amacıyla; Mütercim Tercümanlık, Çeviribilim ve Uygulamalı İngilizce Çevirmenlik öğrencilerine ve mezunlarına gönüllü olarak eğitimler sunuyorum.</p>
      
      <div class="quote">
        <strong>SDL Trados Studio</strong> (CAT yazılımları) ve <strong>Subtitle Edit</strong> gibi araçlara yönelik pratik atölyeler. Bilgisayar destekli çeviri iş akışları ve teknik adaptasyon.
      </div>

      <div class="cta-group">
        <p style="flex: 1; color: var(--muted); font-size: 0.9rem;">Planlanan Zoom atölyeleri için iletişime geçebilirsiniz.</p>
        <a href="mailto:enveradali195@gmail.com?subject=Ücretsiz%20Atölye%20Talebi" class="btn btn-success">
          🎧 Atölye Talep Et
        </a>
      </div>
    </section>

    <!-- KURUMSAL BAĞLANTILAR -->
    <section class="section">
      <h2>Kurumsal Bağlantılar</h2>
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
      <h3 style="margin-top: 0;">📚 Kaynaklar Merkezi</h3>
      <p style="color: var(--muted); margin-bottom: 1.5rem;">Derlem (korpus) veri tabanları, collocation sözlükleri, dinleme platformları ve dikte alıştırmaları.</p>
      <a href="/kaynaklar/" class="btn btn-outline">
        Kaynakları Görüntüle →
      </a>
    </section>

  </div>

  <!-- FOOTER -->
  <footer id="iletisim">
    <div class="footer-container">
      <div class="footer-section">
        <h4>İletişim</h4>
        <div class="footer-contact">
          <strong>E-posta:</strong>
          <a href="mailto:enveradali195@gmail.com">enveradali195@gmail.com</a>
          <br><br>
          <strong>Ağ & İletişim:</strong>
          <a href="https://www.linkedin.com/in/enver-adalı-195" target="_blank" rel="noopener noreferrer">LinkedIn Profili</a>
        </div>
      </div>

      <div class="footer-section">
        <h4>Sayfalar</h4>
        <ul>
          <li><a href="#ana-sayfa">Ana Sayfa</a></li>
          <li><a href="#hakkinda">Perspektif</a></li>
          <li><a href="#dersler">Özel Ders</a></li>
          <li><a href="/kaynaklar/">Kaynaklar & İletişim Formu</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h4>Hizmetler & Odak</h4>
        <ul>
          <li><a href="#dersler">Birebir Özel Ders</a></li>
          <li><a href="#dersler">LGS & Okul Takviyesi</a></li>
          <li><a href="#dersler">Akademik Sınavlar (YDS / TOEFL)</a></li>
          <li><a href="#hakkinda">Gönüllü CAT Araçları Atölyesi</a></li>
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
    const hamburger = document.querySelector('.hamburger');
    const navMenu = document.querySelector('.nav-menu');

    hamburger.addEventListener('click', () => {
      navMenu.classList.toggle('active');
    });

    document.querySelectorAll('.nav-menu a').forEach(link => {
      link.addEventListener('click', () => {
        navMenu.classList.remove('active');
      });
    });
  </script>

  <!-- GİZLİ COĞRAFİ VE AKADEMİK SCHEMA KODU -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "EducationalOccupationalCredential",
    "name": "Birebir ve Online İngilizce Özel Ders",
    "description": "Akademik sınavlara (YDS, TOEFL, LGS) ve dil yeterliliğine yönelik birebir ve online İngilizce eğitimi.",
    "provider": {
      "@type": "Person",
      "name": "Enver Adalı",
      "url": "https://adalienver.site",
      "address": {
        "@type": "PostalAddress",
        "addressRegion": "İstanbul",
        "postalCode": "34570",
        "addressCountry": "TR"
      },
      "geo": {
        "@type": "GeoCoordinates",
        "latitude": 41.0742,
        "longitude": 28.2483
      }
    },
    "areaServed": {
      "@type": "GeoCircle",
      "geoMidpoint": {
        "@type": "GeoCoordinates",
        "latitude": 41.0742,
        "longitude": 28.2483
      },
      "geoRadius": 35000
    },
    "availableChannel": {
      "@type": "ServiceChannel",
      "serviceUrl": "https://adalienver.site",
      "serviceType": "Online Education"
    }
  }
    
  </script>

</body>
</html>
