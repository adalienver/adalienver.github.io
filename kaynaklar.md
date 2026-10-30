---
layout: default
title: İngilizce Öğrenme Materyalleri ve Faydalı Kaynaklar
permalink: /kaynaklar/
---

<style>
  /* HERO BÖLÜMÜ */
  .resource-hero {
    text-align: center;
    margin-bottom: 2.2rem;
  }
  .resource-hero h1 {
    font-family: 'Cinzel', serif;
    font-size: 2.3rem;
    color: var(--primary);
    margin-bottom: 0.6rem;
    letter-spacing: 0.5px;
  }
  .resource-hero p {
    color: var(--muted);
    font-size: 1.02rem;
    max-width: 720px;
    margin: 0 auto;
    line-height: 1.65;
  }

  /* GELİŞMİŞ ARAMA & FİLTRE PANELİ */
  .filter-panel {
    background: rgba(255, 255, 255, 0.88);
    border: 1px solid rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(14px);
    -webkit-backdrop-filter: blur(14px);
    border-radius: 16px;
    padding: 1.35rem 1.5rem;
    margin-bottom: 2.5rem;
    box-shadow: 0 10px 30px -10px rgba(21, 50, 91, 0.08);
  }

  .search-wrapper {
    position: relative;
    margin-bottom: 1.15rem;
  }
  .search-input {
    width: 100%;
    padding: 0.85rem 1.1rem 0.85rem 2.85rem;
    font-size: 0.96rem;
    border: 1px solid var(--border);
    border-radius: 10px;
    outline: none;
    font-family: inherit;
    background: #ffffff;
    transition: all 0.25s ease;
    box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.03);
  }
  .search-input:focus {
    border-color: var(--primary);
    box-shadow: 0 0 0 3px rgba(21, 50, 91, 0.12);
  }
  .search-icon {
    position: absolute;
    left: 1rem;
    top: 50%;
    transform: translateY(-50%);
    color: var(--muted);
    font-size: 1.05rem;
    pointer-events: none;
  }

  .filter-chips {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
  }
  .chip-btn {
    background: #ffffff;
    border: 1px solid var(--border);
    padding: 0.42rem 0.95rem;
    border-radius: 999px;
    font-size: 0.82rem;
    font-weight: 500;
    color: var(--text);
    cursor: pointer;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
  }
  .chip-btn:hover {
    border-color: var(--primary);
    color: var(--primary);
    transform: translateY(-1px);
  }
  .chip-btn.active {
    background: var(--primary);
    color: #ffffff;
    border-color: var(--primary);
    box-shadow: 0 4px 10px rgba(21, 50, 91, 0.2);
  }

  /* KATEGORİ VE KART DÜZENİ */
  .category-title {
    display: flex;
    align-items: center;
    gap: 0.65rem;
    font-family: 'Lora', serif;
    font-size: 1.35rem;
    color: var(--primary);
    margin-bottom: 1.15rem;
    border-bottom: 2px solid rgba(0, 0, 0, 0.05);
    padding-bottom: 0.55rem;
  }

  .resource-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(360px, 1fr));
    gap: 1.2rem;
    margin-bottom: 2.5rem;
  }

  .res-card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: rgba(255, 255, 255, 0.92) !important;
    border: 1px solid rgba(226, 232, 240, 0.9);
    border-radius: 14px;
    padding: 1.4rem 1.5rem;
    text-decoration: none;
    color: var(--text) !important;
    transition: all 0.25s cubic-bezier(0.16, 1, 0.3, 1);
    box-shadow: 0 4px 12px rgba(21, 50, 91, 0.03);
    position: relative;
    overflow: hidden;
  }

  /* Kart sol kenarındaki şık vurgu çizgisi */
  .res-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 4px;
    height: 100%;
    background: transparent;
    transition: background 0.25s ease;
  }
  .res-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 28px rgba(21, 50, 91, 0.09);
    border-color: #cbd5e1;
  }
  .res-card:hover::before {
    background: var(--accent);
  }

  .res-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 0.6rem;
    margin-bottom: 0.6rem;
  }

  .res-title {
    font-weight: 600;
    font-size: 1.05rem;
    color: var(--primary);
    line-height: 1.35;
  }

  .res-desc {
    font-size: 0.88rem;
    color: #4b5563;
    line-height: 1.62;
    margin-bottom: 1.15rem;
  }

  /* ETİKETLER */
  .tag-badge {
    font-size: 0.73rem;
    font-weight: 600;
    padding: 0.25rem 0.65rem;
    border-radius: 999px;
    white-space: nowrap;
    letter-spacing: 0.3px;
  }
  .tag-grammar  { background: #e0f2fe; color: #0369a1; }
  .tag-vocab    { background: #fef3c7; color: #b45309; }
  .tag-reading  { background: #dcfce7; color: #15803d; }
  .tag-audio    { background: #f3e8ff; color: #7e22ce; }
  .tag-youtube  { background: #fee2e2; color: #b91c1c; }
  .tag-official { background: #ede9fe; color: #6d28d9; }
  .tag-corpus   { background: #e0e7ff; color: #3730a3; }
  .tag-context  { background: #fae8ff; color: #86198f; }
  .tag-academic { background: #ffedd5; color: #c2410c; }

  .res-footer {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    font-size: 0.83rem;
    font-weight: 600;
    color: var(--accent);
    gap: 0.3rem;
  }
  .res-footer span {
    transition: transform 0.2s ease;
  }
  .res-card:hover .res-footer span {
    transform: translateX(3px);
  }

  #no-results-msg {
    display: none;
    text-align: center;
    padding: 3rem 1.5rem;
    color: var(--muted);
    font-size: 1rem;
    background: rgba(255, 255, 255, 0.7);
    border-radius: 12px;
    border: 1px dashed var(--border);
  }

  @media (max-width: 640px) {
    .resource-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="resource-hero">
  <h1>İngilizce Öğrenme & Çalışma Kaynakları</h1>
  <p>
    Öğrenciler, çevirmen adayları, lisansüstü araştırmacılar ve dil sınavlarına (YDS, YÖKDİL, TOEFL, IELTS) hazırlananlar için derlenmiş korpus veri tabanları, dinleme ve telaffuz arşivleri, sözlükler ile akademik yazım kılavuzları.
  </p>
</div>

<!-- CANLI FİLTRELEME & ARAMA ÇUBUĞU -->
<div class="filter-panel">
  <div class="search-wrapper">
    <span class="search-icon">🔍</span>
    <input type="text" id="resourceSearch" class="search-input" placeholder="Kaynak adı, konu veya etiket arayın (örn. Korpus, Collocation, Dikte, Bağlaç)..." />
  </div>
  <div class="filter-chips">
    <button class="chip-btn active" data-category="all">Tümü</button>
    <button class="chip-btn" data-category="corpus">🔍 Korpus & Çeviri Belleği</button>
    <button class="chip-btn" data-category="vocab">📚 Eşdizim & Sözlükler</button>
    <button class="chip-btn" data-category="audio">🎧 Dinleme & Telaffuz</button>
    <button class="chip-btn" data-category="grammar">📘 Dilbilgisi & Yapı</button>
    <button class="chip-btn" data-category="academic">🎓 Akademik Yazım</button>
    <button class="chip-btn" data-category="reading">📖 Okuma & Test</button>
  </div>
</div>

<div id="no-results-msg">Aradığınız kritere uygun kaynak bulunamadı. Lütfen farklı bir arama sözcüğü deneyin.</div>

<!-- 1. KORPUS & ÇEVİRİ BELLEĞİ -->
<div class="category-section" data-section="corpus">
  <h2 class="category-title">🔍 Korpus, Bağlamsal Arama & Çeviri Veri Tabanları</h2>
  <div class="resource-grid">

    <a href="https://www.english-corpora.org/coca/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="coca corpus contemporary american english akademik dilbilim derlem eşdizim frekans sıklık">
      <div>
        <div class="res-header">
          <span class="res-title">COCA (Corpus of Contemporary American)</span>
          <span class="tag-badge tag-corpus">Akademik Korpus</span>
        </div>
        <p class="res-desc">
          Milyarlarca kelimelik devasa veri tabanıyla bir sözcüğün akademik makalelerde, edebiyatta veya basında nasıl kullanıldığını ve hangi kalıplarla eşleştiğini görmenizi sağlar.
        </p>
      </div>
      <div class="res-footer">Korpusu İncele <span>↗</span></div>
    </a>

    <a href="https://ludwig.guru/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="ludwig guru cümle doğrulama muteber kaynak nyt guardian context bağlamsal arama">
      <div>
        <div class="res-header">
          <span class="res-title">Ludwig.guru</span>
          <span class="tag-badge tag-context">Cümle Doğrulama</span>
        </div>
        <p class="res-desc">
          Yazdığınız İngilizce cümlenin doğal olup olmadığını The New York Times, BBC veya bilimsel makalelerdeki gerçek örneklerle kıyaslayarak teyit eden pratik bir arama motoru.
        </p>
      </div>
      <div class="res-footer">Cümleyi Test Et <span>↗</span></div>
    </a>

    <a href="https://dictionary.reverso.net/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="reverso context dictionary çeviri paralel metin sözlük iki dilli">
      <div>
        <div class="res-header">
          <span class="res-title">Reverso Context & Dictionary</span>
          <span class="tag-badge tag-context">Bağlam Çevirisi</span>
        </div>
        <p class="res-desc">
          Kelimeleri ve kalıpları bağlamından koparmadan, milyonlarca iki dilli gerçek çeviri cümlesi içinde yan yana görmenizi sağlayan çevirmen dostu bir platform.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç <span>↗</span></div>
    </a>

    <a href="https://sentencedict.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="sentencedict cümle arama örnek cümle bağlam context örnekler">
      <div>
        <div class="res-header">
          <span class="res-title">SentenceDict</span>
          <span class="tag-badge tag-context">Örnek Cümleler</span>
        </div>
        <p class="res-desc">
          Aranan kelimenin farklı seviyelerdeki hazır cümlelerde nasıl yer aldığını derli toplu listeleyen hızlı bir örnekleme aracı.
        </p>
      </div>
      <div class="res-footer">Cümle Bul <span>↗</span></div>
    </a>

    <a href="https://glosbe.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="glosbe çok dilli bellek translation memory paralel corpus terim çevirisi">
      <div>
        <div class="res-header">
          <span class="res-title">Glosbe Paralel Bellek</span>
          <span class="tag-badge tag-corpus">Paralel Metinler</span>
        </div>
        <p class="res-desc">
          Farklı dillerdeki resmi ve sektörel çevirileri eşleştiren, özellikle terim çevirilerinde güvenilir karşılıklar bulmaya yarayan geniş bir bellek sözlüğü.
        </p>
      </div>
      <div class="res-footer">Glosbe'yi Aç <span>↗</span></div>
    </a>

  </div>
</div>

<!-- 2. EŞDİZİM & SÖZLÜKLER -->
<div class="category-section" data-section="vocab">
  <h2 class="category-title">📚 Eşdizim (Collocation) & İleri Düzey Sözlükler</h2>
  <div class="resource-grid">

    <a href="https://ozdic.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="ozdic collocations eşdizim sözlük preposition edat fiil tamlama doğal kullanım">
      <div>
        <div class="res-header">
          <span class="res-title">Ozdic Collocations Dictionary</span>
          <span class="tag-badge tag-vocab">Çevirmen Başucu</span>
        </div>
        <p class="res-desc">
          İngilizcede hangi kelimenin hangi fiil, sıfat veya edatla kalıp türettiğini (make a decision, heavy rain gibi) gösteren temel başvuru kaynağı.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç <span>↗</span></div>
    </a>

    <a href="https://www.just-the-word.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="just the word lextra collocations bnc british national corpus eşdizim denetimi">
      <div>
        <div class="res-header">
          <span class="res-title">Just The Word (BNC Tabanlı)</span>
          <span class="tag-badge tag-vocab">Eşdizim Analizi</span>
        </div>
        <p class="res-desc">
          İngilizce Külliyatı  verilerini temel alan kelime eşleşmelerinin sıklığını ve kullanım sıklığını s.
        </p>
      </div>
      <div class="res-footer">Analizi Başlat <span>↗</span></div>
    </a>

    <a href="https://www.wordhippo.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="wordhippo eş anlam zıt anlam thesaurus bağlam kafiye kelime dağarcığı">
      <div>
        <div class="res-header">
          <span class="res-title">WordHippo</span>
          <span class="tag-badge tag-vocab">Kapsamlı Thesaurus</span>
        </div>
        <p class="res-desc">
          Aradığınız kelimenin en ince anlamına kadar eşanlamlılarını, zıt anlamlarını, bağlama göre alternatiflerini ve kafiyelerini tek sayfada sunan zengin bir kelime platformu.
        </p>
      </div>
      <div class="res-footer">Kelime İncele <span>↗</span></div>
    </a>

    <a href="https://www.vocabulary.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="vocabulary kelime ezber bağlam akıllı alıştırma ileri düzey">
      <div>
        <div class="res-header">
          <span class="res-title">Vocabulary.com</span>
          <span class="tag-badge tag-vocab">Akıllı Kelime Motoru</span>
        </div>
        <p class="res-desc">
          Kelimeleri ezberletmek yerine hikâyeleri, edebi kullanımları ve akıllı soru sistemiyle zihinde kalıcı hale getiren etkileşimli bir öğrenme alanı.
        </p>
      </div>
      <div class="res-footer">Kelime Çalış <span>↗</span></div>
    </a>

    <a href="https://www.thefreedictionary.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="the free dictionary farlex terim sözlük hukuk tıp idari deyim">
      <div>
        <div class="res-header">
          <span class="res-title">The Free Dictionary (Farlex)</span>
          <span class="tag-badge tag-vocab">Uzmanlık Alanları</span>
        </div>
        <p class="res-desc">
          Genel sözlüklerin ötesine geçerek hukuk, tıp, iktisat terimlerini ve kısaltmaları bir araya toplayan devasa bir dijital başvuru kütüphanesi.
        </p>
      </div>
      <div class="res-footer">Portalda Ara <span>↗</span></div>
    </a>

    <a href="https://www.eslcafe.com/resources/idioms" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="esl cafe dave idioms deyimler kalıplar sokak dili günlük konuşma">
      <div>
        <div class="res-header">
          <span class="res-title">Dave's ESL Cafe: Idioms</span>
          <span class="tag-badge tag-vocab">Deyim Arşivi</span>
        </div>
        <p class="res-desc">
          İngilizcede gündelik hayatın ve sokak dilinde yaygın olan, net açıklamalar ve gerçek hayat örnekleriyle alfabetik olarak sıralayan klasik bir arşiv.
        </p>
      </div>
      <div class="res-footer">Deyimleri İncele <span>↗</span></div>
    </a>

  </div>
</div>

<!-- 3. DİNLEME, HABER & TELAFFUZ -->
<div class="category-section" data-section="audio">
  <h2 class="category-title">🎧 Dinleme (Listening), Haber & Canlı Telaffuz</h2>
  <div class="resource-grid">

    <a href="https://youglish.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="youglish youtube telaffuz aksan british american australian canlı örnek">
      <div>
        <div class="res-header">
          <span class="res-title">YouGlish: Contextual Pronunciation</span>
          <span class="tag-badge tag-youtube">Canlı Telaffuz</span>
        </div>
        <p class="res-desc">
          Yazdığınız herhangi bir ifadenin YouTube videolarında gerçek insanlar tarafından Amerikan, İngiliz veya Avustralya aksanlarıyla nasıl seslendirildiğini anında önünüze getiren benzersiz bir araç.
        </p>
      </div>
      <div class="res-footer">Telaffuz Dinle <span>↗</span></div>
    </a>

    <a href="https://www.bbc.co.uk/learningenglish/english/features/6-minute-english" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="bbc 6 minute english podcast haber dinleme listening transcript metin">
      <div>
        <div class="res-header">
          <span class="res-title">BBC: 6 Minute English Arşivi</span>
          <span class="tag-badge tag-official">Podcast & Transkript</span>
        </div>
        <p class="res-desc">
          Her bölümde altı dakikalık  konular işleyen, kelime listeleri ve tam metin dökümleriyle dinleme pratiği içeren pdocast serisi.
        </p>
      </div>
      <div class="res-footer">Bölümleri Dinle <span>↗</span></div>
    </a>

    <a href="https://learningenglish.voanews.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="voa learning english voice of america haber dikte dinleme listening sade dil">
      <div>
        <div class="res-header">
          <span class="res-title">VOA Learning English</span>
          <span class="tag-badge tag-audio">Ses & Yavaş Haber</span>
        </div>
        <p class="res-desc">
          Normalden  bir tempoyla  seslendirilen dünya haberleri, shadowing çalışmaları için .
        </p>
      </div>
      <div class="res-footer">Haberleri İncele <span>↗</span></div>
    </a>

    <a href="https://www.youtube.com/@engvidRonnie/videos" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="engvid ronnie video youtube konuşma argo slang gramer video ders">
      <div>
        <div class="res-header">
          <span class="res-title">engVid: Ronnie’s English Channel</span>
          <span class="tag-badge tag-youtube">Video Ders</span>
        </div>
        <p class="res-desc">
          Kitabi kurallardan dışında, günlük yaşamın sokak dilini, esprileri ve kafa karıştıran dilbilgisi nüancslarını samimi  bir üslupla ele alan İngilizce  dersler.
        </p>
      </div>
      <div class="res-footer">Kanala Git <span>↗</span></div>
    </a>

    <a href="https://learnenglish.britishcouncil.org/free-resources" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="british council ielts podcast sınav hazırlık iş ingilizcesi dinleme alıştırma">
      <div>
        <div class="res-header">
          <span class="res-title">British Council: Podcasts & Resources</span>
          <span class="tag-badge tag-official">Kurumsal / Sınav</span>
        </div>
        <p class="res-desc">
          Temel seviyeden ileri düzeye kadar yapılandırılmış ses kayıtları, IELTS hazırlık ipuçları ve mesleki İngilizceye yönelik kapsamlı alıştırma seti.
        </p>
      </div>
      <div class="res-footer">Materyalleri Aç <span>↗</span></div>
    </a>

  </div>
</div>

<!-- 4. AKADEMİK YAZIM & MAKALE STANDARTLARI -->
<div class="category-section" data-section="academic">
  <h2 class="category-title">🎓 Akademik Yazım, Metin Mimarisi & APA/MLA</h2>
  <div class="resource-grid">

    <a href="https://owl.purdue.edu/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="academic" data-keywords="purdue owl online writing lab akademik yazım apa mla alıntı essay thesis tez makale">
      <div>
        <div class="res-header">
          <span class="res-title">Purdue OWL (Online Writing Lab)</span>
          <span class="tag-badge tag-academic">Akademik Standart</span>
        </div>
        <p class="res-desc">
          Tez, makale ve akademik yazımlarda  argüman, paragraf yapısı ile APA ve MLA kaynak  standartlarında  bir rehber.
        </p>
      </div>
      <div class="res-footer">Kılavuza Git <span>↗</span></div>
    </a>

    <a href="https://www.phrasebank.manchester.ac.uk/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="academic" data-keywords="manchester academic phrasebank akademik kalıplar makale yazımı tez giriş sonuç tartışma literatür">
      <div>
        <div class="res-header">
          <span class="res-title">Manchester Academic Phrasebank</span>
          <span class="tag-badge tag-academic">Akademik Kalıplar</span>
        </div>
        <p class="res-desc">
          Akademik metinlerin yazımında gerekli ifadeler ve bilinmesi gereken kalıplar.
        </p>
      </div>
      <div class="res-footer">Kalıpları İncele <span>↗</span></div>
    </a>

  </div>
</div>

<!-- 5. DİLBİLGİSİ & CÜMLE MİMARİSİ -->
<div class="category-section" data-section="grammar">
  <h2 class="category-title">📘 Dilbilgisi & Cümle Mimarisi</h2>
  <div class="resource-grid">

    <a href="https://dictionary.cambridge.org/grammar/british-grammar/conjunctions-time" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="cambridge grammar conjunctions bağlaçlar zaman clauses syntax yan tümce">
      <div>
        <div class="res-header">
          <span class="res-title">Cambridge Grammar: Conjunctions</span>
          <span class="tag-badge tag-grammar">Bağlaçlar</span>
        </div>
        <p class="res-desc">
          Zaman bağlaçları, yan cümleler ve metin içi mantıksal geçişlerin doğru kullanımı üzerine Cambridge güvencesiyle hazırlanmış ayrıntılı bir kaynak.
        </p>
      </div>
      <div class="res-footer">Kılavuzu Oku <span>↗</span></div>
    </a>

    <a href="https://www.engvid.com/english-resource/verbs-followed-by-gerunds-and-infinitives/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="gerund infinitive engvid fiil yapıları verb structures ing to infinitives">
      <div>
        <div class="res-header">
          <span class="res-title">EngVid: Gerunds & Infinitives Table</span>
          <span class="tag-badge tag-grammar">Fiil Yapıları</span>
        </div>
        <p class="res-desc">
          Hangi fiilden sonra "-ing", hangisinden sonra "to" geldiğini net ayrımlarla ve örneklerle gösteren pratik bir başvuru tablosu.
        </p>
      </div>
      <div class="res-footer">Tabloyu İncele <span>↗</span></div>
    </a>

    <a href="https://www.ef.com/wwen/english-resources/english-grammar/pick-right-quantifier/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="ef quantifiers miktar belirteçleri much many few little sayılabilen isimler">
      <div>
        <div class="res-header">
          <span class="res-title">EF English: Pick the Right Quantifier</span>
          <span class="tag-badge tag-grammar">Miktar Belirteçleri</span>
        </div>
        <p class="res-desc">
          Much/many, few/little gibi sayılabilen ve sayılamayan isimlerle kullanılan belirteçlerin ayrımını yalın örneklerle açıklayan rehber.
        </p>
      </div>
      <div class="res-footer">Rehbere Git <span>↗</span></div>
    </a>

    <a href="https://www.englishclub.com/grammar/determiners-quantifiers.php" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="englishclub determiners quantifiers alıştırma test soruları kurallar">
      <div>
        <div class="res-header">
          <span class="res-title">EnglishClub: Determiners</span>
          <span class="tag-badge tag-grammar">Referans</span>
        </div>
        <p class="res-desc">
          Belirteç sistemini sade kurallar, test soruları ve en sık yapılan hatalar üzerinden pratik yaptıran faydalı bir çalışma sayfası.
        </p>
      </div>
      <div class="res-footer">Alıştırmaları Gör <span>↗</span></div>
    </a>

  </div>
</div>

<!-- 6. OKUMA PRATİĞİ & TESTLER -->
<div class="category-section" data-section="reading">
  <h2 class="category-title">📖 Okuma Kavrama & Seviye Testleri</h2>
  <div class="resource-grid">

    <a href="https://test-english.com/reading/a1/guess-who-a1-english-reading-test/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="reading" data-keywords="test english reading a1 okuma kavrama seviye sınavı test değerlendirme">
      <div>
        <div class="res-header">
          <span class="res-title">Test-English: A1 Reading Test</span>
          <span class="tag-badge tag-reading">Seviye Testi</span>
        </div>
        <p class="res-desc">
          Başlangıç düzeyindeki okuma parçaları ve anında dönüt veren testleriyle temel kavrama becerilerini ölçen pratik bir çalışma alanı.
        </p>
      </div>
      <div class="res-footer">Testi Çöz <span>↗</span></div>
    </a>

    <a href="https://lingua.com/english/reading/wonderful-family/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="reading" data-keywords="lingua reading practice metin okuma parça sorular değerlendirme öykü">
      <div>
        <div class="res-header">
          <span class="res-title">Lingua: English Reading Practice</span>
          <span class="tag-badge tag-reading">Metin Okuma</span>
        </div>
        <p class="res-desc">
          Farklı seviyelere göre ayrılmış kısa öykü ve metinler üzerinden okuma hızını ve anlama yetisini geliştiren sorular içeren bir portal.
        </p>
      </div>
      <div class="res-footer">Metinleri Oku <span>↗</span></div>
    </a>

  </div>
</div>

<!-- ANINDA FİLTRELEME VE ARAMA JAVASCRIPT KODU -->
<script>
  (function() {
    const searchInput = document.getElementById('resourceSearch');
    const chipBtns = document.querySelectorAll('.chip-btn');
    const sections = document.querySelectorAll('.category-section');
    const noResults = document.getElementById('no-results-msg');

    let activeCategory = 'all';

    function filterResources() {
      const query = searchInput.value.toLowerCase().trim();
      let visibleTotal = 0;

      sections.forEach(sec => {
        let sectionVisibleCount = 0;
        const secCards = sec.querySelectorAll('.res-card');

        secCards.forEach(card => {
          const cat = card.getAttribute('data-category');
          const keywords = (card.getAttribute('data-keywords') || '').toLowerCase();
          const text = card.textContent.toLowerCase();

          const matchesCat = (activeCategory === 'all' || cat === activeCategory);
          const matchesQuery = (query === '' || text.includes(query) || keywords.includes(query));

          if (matchesCat && matchesQuery) {
            card.style.display = 'flex';
            sectionVisibleCount++;
            visibleTotal++;
          } else {
            card.style.display = 'none';
          }
        });

        // Başlık altında kart kalmadıysa o kategori başlığını gizle
        sec.style.display = sectionVisibleCount > 0 ? 'block' : 'none';
      });

      noResults.style.display = visibleTotal === 0 ? 'block' : 'none';
    }

    searchInput.addEventListener('input', filterResources);

    chipBtns.forEach(btn => {
      btn.addEventListener('click', () => {
        chipBtns.forEach(b => b.classList.remove('active'));
        btn.classList.add('active');
        activeCategory = btn.getAttribute('data-category');
        filterResources();
      });
    });
  })();
</script>
