---
layout: default
title: İngilizce Çalışma Kaynakları & İnteraktif Testler
description: YDS, YÖKDİL, TOEFL, LGS hazırlığı ve çeviri çalışmaları için korpus veri tabanları, eşdizim sözlükleri, dikte araçları, seviyeli dil testleri ve iletişim formu.
permalink: /kaynaklar/
---

<style>
  /* HERO BÖLÜMÜ (KOMPAKT) */
  .resource-hero {
    text-align: center;
    margin-bottom: 1.5rem;
  }
  .resource-hero h1 {
    font-family: 'Cinzel', serif;
    font-size: 2rem;
    color: var(--primary);
    margin-bottom: 0.45rem;
    letter-spacing: 0.4px;
  }
  .resource-hero p {
    color: var(--muted);
    font-size: 0.94rem;
    max-width: 720px;
    margin: 0 auto;
    line-height: 1.55;
  }

  /* ARAMA & FİLTRE PANELİ (DARALTILMIŞ) */
  .filter-panel {
    background: rgba(255, 255, 255, 0.9);
    border: 1px solid rgba(226, 232, 240, 0.95);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border-radius: 12px;
    padding: 0.95rem 1.15rem;
    margin-bottom: 1.75rem;
    box-shadow: 0 6px 20px -8px rgba(21, 50, 91, 0.08);
  }

  .search-wrapper {
    position: relative;
    margin-bottom: 0.75rem;
  }
  .search-input {
    width: 100%;
    padding: 0.65rem 0.95rem 0.65rem 2.45rem;
    font-size: 0.9rem;
    border: 1px solid var(--border);
    border-radius: 8px;
    outline: none;
    font-family: inherit;
    background: #ffffff;
    transition: all 0.2s ease;
  }
  .search-input:focus {
    border-color: var(--primary);
    box-shadow: 0 0 0 3px rgba(21, 50, 91, 0.1);
  }
  .search-icon {
    position: absolute;
    left: 0.85rem;
    top: 50%;
    transform: translateY(-50%);
    color: var(--muted);
    font-size: 0.95rem;
    pointer-events: none;
  }

  .filter-chips {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    align-items: center;
  }
  .chip-btn,
  .jump-chip {
    background: #ffffff;
    border: 1px solid var(--border);
    padding: 0.32rem 0.75rem;
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 500;
    color: var(--text);
    cursor: pointer;
    transition: all 0.2s ease;
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    text-decoration: none;
  }
  .chip-btn:hover,
  .jump-chip:hover {
    border-color: var(--primary);
    color: var(--primary);
  }
  .chip-btn.active {
    background: var(--primary);
    color: #ffffff;
    border-color: var(--primary);
  }
  .jump-chip {
    background: #fef9f3;
    border-color: var(--accent);
    color: var(--primary);
    font-weight: 600;
    margin-left: auto;
  }

  /* KATEGORİ VE KOMPAKT KART DÜZENİ */
  .category-section {
    margin-bottom: 1.75rem;
  }
  .category-title {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-family: 'Lora', serif;
    font-size: 1.15rem;
    color: var(--primary);
    margin-bottom: 0.8rem;
    border-bottom: 1px solid rgba(0, 0, 0, 0.08);
    padding-bottom: 0.4rem;
  }

  .resource-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(265px, 1fr));
    gap: 0.85rem;
  }

  .res-card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: rgba(255, 255, 255, 0.94) !important;
    border: 1px solid rgba(226, 232, 240, 0.95);
    border-radius: 10px;
    padding: 0.95rem 1.05rem;
    text-decoration: none;
    color: var(--text) !important;
    transition: all 0.2s ease;
    box-shadow: 0 2px 8px rgba(21, 50, 91, 0.03);
    position: relative;
    overflow: hidden;
  }

  .res-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 3px;
    height: 100%;
    background: transparent;
    transition: background 0.2s ease;
  }
  .res-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 18px rgba(21, 50, 91, 0.08);
    border-color: #cbd5e1;
  }
  .res-card:hover::before {
    background: var(--accent);
  }

  .res-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 0.45rem;
    margin-bottom: 0.4rem;
  }

  .res-title {
    font-weight: 600;
    font-size: 0.94rem;
    color: var(--primary);
    line-height: 1.3;
  }

  .res-desc {
    font-size: 0.81rem;
    color: #4b5563;
    line-height: 1.48;
    margin-bottom: 0.65rem;
  }

  /* ETİKETLER */
  .tag-badge {
    font-size: 0.67rem;
    font-weight: 600;
    padding: 0.18rem 0.52rem;
    border-radius: 999px;
    white-space: nowrap;
    letter-spacing: 0.2px;
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
    font-size: 0.77rem;
    font-weight: 600;
    color: var(--accent);
    gap: 0.25rem;
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
    padding: 2rem 1rem;
    color: var(--muted);
    font-size: 0.92rem;
    background: rgba(255, 255, 255, 0.7);
    border-radius: 10px;
    border: 1px dashed var(--border);
    margin-bottom: 1.5rem;
  }

  /* İNTERAKTİF DİL & ÇEVİRİ TESTLERİ BÖLÜMÜ */
  .quiz-section {
    margin-top: 2.5rem;
    padding-top: 1.75rem;
    border-top: 1px solid rgba(0, 0, 0, 0.08);
  }
  .quiz-section-intro {
    color: var(--muted);
    font-size: 0.9rem;
    margin-bottom: 1.1rem;
    line-height: 1.55;
  }
  .tools-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 1.15rem;
  }
  .tool-card {
    background: rgba(255, 255, 255, 0.94);
    border: 1px solid rgba(226, 232, 240, 0.95);
    border-radius: 12px;
    padding: 1.2rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    box-shadow: 0 4px 14px rgba(21, 50, 91, 0.04);
  }
  .tool-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 0.5rem;
    margin-bottom: 0.65rem;
    flex-wrap: wrap;
  }
  .tool-header strong {
    color: var(--primary);
    font-size: 0.98rem;
  }
  .tool-badge {
    font-size: 0.7rem;
    font-weight: 700;
    background: var(--light);
    color: var(--secondary);
    border: 1px solid var(--border);
    padding: 0.18rem 0.55rem;
    border-radius: 999px;
  }
  .tool-sub {
    font-size: 0.82rem;
    color: var(--muted);
    margin-bottom: 0.75rem;
    line-height: 1.45;
  }
  .level-tabs {
    display: flex;
    gap: 0.4rem;
    margin-bottom: 0.75rem;
  }
  .level-tab {
    flex: 1;
    padding: 0.4rem 0.5rem;
    font-size: 0.78rem;
    font-weight: 600;
    border: 1px solid var(--border);
    border-radius: 6px;
    background: #fff;
    color: var(--muted);
    cursor: pointer;
    transition: all 0.2s ease;
  }
  .level-tab:hover {
    border-color: var(--primary);
    color: var(--primary);
  }
  .level-tab.active {
    background: var(--primary);
    color: #fff;
    border-color: var(--primary);
  }
  .quiz-box {
    background: var(--light);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 0.95rem;
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .quiz-top {
    display: flex;
    justify-content: space-between;
    font-size: 0.77rem;
    font-weight: 600;
    color: var(--muted);
    margin-bottom: 0.65rem;
    padding-bottom: 0.4rem;
    border-bottom: 1px solid var(--border);
  }
  .quiz-question {
    font-size: 0.89rem;
    font-weight: 500;
    color: var(--primary);
    margin-bottom: 0.75rem;
    line-height: 1.5;
  }
  .quiz-options {
    display: flex;
    flex-direction: column;
    gap: 0.4rem;
  }
  .quiz-opt-btn {
    text-align: left;
    padding: 0.5rem 0.75rem;
    background: #ffffff;
    border: 1px solid var(--border);
    border-radius: 6px;
    font-size: 0.83rem;
    cursor: pointer;
    transition: all 0.18s ease;
    color: var(--text);
    font-family: inherit;
  }
  .quiz-opt-btn:hover:not(:disabled) {
    border-color: var(--primary);
    background: #f1f5f9;
  }
  .quiz-opt-btn.correct {
    background: #dcfce7;
    border-color: #16a34a;
    color: #14532d;
    font-weight: 600;
  }
  .quiz-opt-btn.wrong {
    background: #fee2e2;
    border-color: #dc2626;
    color: #7f1d1d;
  }
  .quiz-feedback {
    margin-top: 0.65rem;
    font-size: 0.79rem;
    padding: 0.55rem 0.7rem;
    border-radius: 5px;
    background: #ffffff;
    border-left: 3px solid var(--accent);
    color: var(--text);
    line-height: 1.45;
  }
  .quiz-next-btn {
    margin-top: 0.75rem;
    padding: 0.48rem 1rem;
    font-size: 0.82rem;
    font-weight: 600;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    background: var(--primary);
    color: #ffffff;
    align-self: flex-start;
  }
  .quiz-next-btn.secondary {
    background: var(--accent);
  }

  /* İLETİŞİM FORMU BÖLÜMÜ */
  .resource-contact-section {
    margin-top: 2.75rem;
    padding-top: 1.75rem;
    border-top: 1px solid rgba(0, 0, 0, 0.08);
  }
  .contact-box {
    background: rgba(255, 255, 255, 0.94);
    border: 1px solid rgba(226, 232, 240, 0.95);
    border-top: 3px solid var(--accent);
    border-radius: 14px;
    padding: 1.65rem;
    max-width: 680px;
    margin: 0 auto;
    box-shadow: 0 8px 24px -10px rgba(21, 50, 91, 0.06);
  }
  .contact-box p {
    color: #4b5563;
    font-size: 0.89rem;
    line-height: 1.55;
    margin-bottom: 1.2rem;
  }
  .custom-contact-form {
    display: flex;
    flex-direction: column;
    gap: 0.95rem;
  }
  .form-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.9rem;
  }
  .form-group {
    display: flex;
    flex-direction: column;
    gap: 0.35rem;
  }
  .form-group label {
    font-size: 0.84rem;
    font-weight: 600;
    color: var(--primary);
  }
  .form-group input,
  .form-group select,
  .form-group textarea {
    width: 100%;
    padding: 0.68rem 0.85rem;
    border: 1px solid var(--border);
    border-radius: 8px;
    font-size: 0.89rem;
    background: #ffffff;
    color: var(--text);
    box-sizing: border-box;
    font-family: inherit;
    transition: all 0.2s ease;
  }
  .form-group input:focus,
  .form-group select:focus,
  .form-group textarea:focus {
    outline: none;
    border-color: var(--primary);
    box-shadow: 0 0 0 3px rgba(21, 50, 91, 0.1);
  }
  .submit-btn {
    background: var(--primary);
    color: #ffffff;
    padding: 0.72rem 1.5rem;
    font-size: 0.9rem;
    font-weight: 600;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    align-self: flex-start;
    transition: all 0.2s ease;
  }
  .submit-btn:hover {
    background: #0f2442;
    transform: translateY(-1px);
  }
  .internal-links-bar {
    margin-top: 1.35rem;
    padding-top: 1rem;
    border-top: 1px solid var(--border);
    font-size: 0.82rem;
    color: var(--muted);
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem 1rem;
    justify-content: center;
  }
  .internal-links-bar a {
    color: var(--primary);
    font-weight: 600;
    text-decoration: none;
  }
  .internal-links-bar a:hover {
    color: var(--accent);
    text-decoration: underline;
  }

  @media (max-width: 640px) {
    .resource-grid,
    .tools-grid,
    .form-row {
      grid-template-columns: 1fr;
    }
    .jump-chip {
      margin-left: 0;
    }
    .contact-box {
      padding: 1.25rem;
    }
  }
</style>

<div class="resource-hero">
  <h1>İngilizce Çalışma Kaynakları & Testler</h1>
  <p>
    Öğrenciler, çevirmen adayları ve dil sınavlarına hazırlananlar için derlenmiş korpus veri tabanları, eşdizim sözlükleri, dinleme arşivleri, akademik yazım kılavuzları ve etkileşimli alıştırmalar.
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
    <button class="chip-btn" data-category="corpus">🔍 Korpus & Bellek</button>
    <button class="chip-btn" data-category="vocab">📚 Eşdizim & Sözlük</button>
    <button class="chip-btn" data-category="audio">🎧 Dinleme & Telaffuz</button>
    <button class="chip-btn" data-category="grammar">📘 Dilbilgisi</button>
    <button class="chip-btn" data-category="academic">🎓 Akademik Yazım</button>
    <button class="chip-btn" data-category="reading">📖 Okuma</button>
    <a href="#interaktif-testler" class="jump-chip">⚡ Bağlaç & Çeviri Testleri ↓</a>
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
          <span class="res-title">COCA (American Corpus)</span>
          <span class="tag-badge tag-corpus">Korpus</span>
        </div>
        <p class="res-desc">
          Milyarlarca kelimelik veri tabanıyla sözcüklerin akademik makalelerde, edebiyatta ve basındaki kullanım sıklığını ve kalıplarını gösterir.
        </p>
      </div>
      <div class="res-footer">Korpusu İncele <span>↗</span></div>
    </a>

    <a href="https://ludwig.guru/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="ludwig guru cümle doğrulama muteber kaynak nyt guardian context bağlamsal arama">
      <div>
        <div class="res-header">
          <span class="res-title">Ludwig.guru</span>
          <span class="tag-badge tag-context">Doğrulama</span>
        </div>
        <p class="res-desc">
          Yazdığınız İngilizce cümlenin doğal olup olmadığını The New York Times, BBC ve akademik yayınlardaki gerçek örneklerle kıyaslar.
        </p>
      </div>
      <div class="res-footer">Cümleyi Test Et <span>↗</span></div>
    </a>

    <a href="https://dictionary.reverso.net/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="reverso context dictionary çeviri paralel metin sözlük iki dilli">
      <div>
        <div class="res-header">
          <span class="res-title">Reverso Context</span>
          <span class="tag-badge tag-context">Bağlam</span>
        </div>
        <p class="res-desc">
          Kelimeleri ve kalıpları bağlamından koparmadan milyonlarca iki dilli gerçek çeviri cümlesi içinde yan yana sunan çevirmen aracı.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç <span>↗</span></div>
    </a>

    <a href="https://sentencedict.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="sentencedict cümle arama örnek cümle bağlam context örnekler">
      <div>
        <div class="res-header">
          <span class="res-title">SentenceDict</span>
          <span class="tag-badge tag-context">Örnek Cümle</span>
        </div>
        <p class="res-desc">
          Aranan kelimenin farklı zorluk düzeylerindeki hazır cümlelerde nasıl yer aldığını hızlıca listeleyen pratik örnekleme aracı.
        </p>
      </div>
      <div class="res-footer">Cümle Bul <span>↗</span></div>
    </a>

    <a href="https://glosbe.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="glosbe çok dilli bellek translation memory paralel corpus terim çevirisi">
      <div>
        <div class="res-header">
          <span class="res-title">Glosbe Paralel Bellek</span>
          <span class="tag-badge tag-corpus">Bellek</span>
        </div>
        <p class="res-desc">
          Farklı dillerdeki resmi ve sektörel çevirileri eşleştiren, terim çevirilerinde güvenilir karşılıklar sunan geniş paralel metin sözlüğü.
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
          <span class="res-title">Ozdic Collocations</span>
          <span class="tag-badge tag-vocab">Eşdizim</span>
        </div>
        <p class="res-desc">
          Hangi sözcüğün hangi fiil, sıfat veya edatla doğal kalıp kurduğunu (make a decision, heavy rain gibi) gösteren temel başvuru sözlüğü.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç <span>↗</span></div>
    </a>

    <a href="https://www.just-the-word.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="just the word lextra collocations bnc british national corpus eşdizim denetimi">
      <div>
        <div class="res-header">
          <span class="res-title">Just The Word (BNC)</span>
          <span class="tag-badge tag-vocab">Analiz</span>
        </div>
        <p class="res-desc">
          İngiliz Ulusal Külliyatı (BNC) verilerini kullanarak kelime eşleşmelerinin kullanım sıklığını ve doğallığını puanlayan analitik araç.
        </p>
      </div>
      <div class="res-footer">Analizi Başlat <span>↗</span></div>
    </a>

    <a href="https://www.wordhippo.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="wordhippo eş anlam zıt anlam thesaurus bağlam kafiye kelime dağarcığı">
      <div>
        <div class="res-header">
          <span class="res-title">WordHippo</span>
          <span class="tag-badge tag-vocab">Thesaurus</span>
        </div>
        <p class="res-desc">
          Aradığınız kelimenin ince anlam farklarına göre eşanlamlılarını, zıt anlamlarını ve bağlamsal alternatiflerini tek sayfada sunar.
        </p>
      </div>
      <div class="res-footer">Kelime İncele <span>↗</span></div>
    </a>

    <a href="https://www.vocabulary.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="vocabulary kelime ezber bağlam akıllı alıştırma ileri düzey">
      <div>
        <div class="res-header">
          <span class="res-title">Vocabulary.com</span>
          <span class="tag-badge tag-vocab">Kelime</span>
        </div>
        <p class="res-desc">
          Kelimeleri ezberletmek yerine edebi kullanımlar, kısa açıklamalar ve uyarlanabilir soru sistemiyle kalıcı hale getiren platform.
        </p>
      </div>
      <div class="res-footer">Kelime Çalış <span>↗</span></div>
    </a>

    <a href="https://www.thefreedictionary.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="the free dictionary farlex terim sözlük hukuk tıp idari deyim">
      <div>
        <div class="res-header">
          <span class="res-title">The Free Dictionary</span>
          <span class="tag-badge tag-vocab">Terim</span>
        </div>
        <p class="res-desc">
          Genel sözlüklerin ötesinde hukuk, tıp, iktisat terimlerini ve kısaltmaları bir araya getiren kapsamlı dijital başvuru kaynağı.
        </p>
      </div>
      <div class="res-footer">Portalda Ara <span>↗</span></div>
    </a>

    <a href="https://www.eslcafe.com/resources/idioms" target="_blank" rel="noopener noreferrer" class="res-card" data-category="vocab" data-keywords="esl cafe dave idioms deyimler kalıplar sokak dili günlük konuşma">
      <div>
        <div class="res-header">
          <span class="res-title">Dave's ESL Cafe: Idioms</span>
          <span class="tag-badge tag-vocab">Deyimler</span>
        </div>
        <p class="res-desc">
          Gündelik konuşmada ve anlatımda sık geçen İngilizce deyimleri net açıklamalar ve örnek cümlelerle sıralayan klasik arşiv.
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
          <span class="res-title">YouGlish Pronunciation</span>
          <span class="tag-badge tag-youtube">Telaffuz</span>
        </div>
        <p class="res-desc">
          Yazdığınız ifadenin YouTube videolarında Amerikan, İngiliz veya Avustralya aksanlarıyla gerçek kişilerce nasıl telaffuz edildiğini gösterir.
        </p>
      </div>
      <div class="res-footer">Telaffuz Dinle <span>↗</span></div>
    </a>

    <a href="https://www.bbc.co.uk/learningenglish/english/features/6-minute-english" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="bbc 6 minute english podcast haber dinleme listening transcript metin">
      <div>
        <div class="res-header">
          <span class="res-title">BBC: 6 Minute English</span>
          <span class="tag-badge tag-official">Podcast</span>
        </div>
        <p class="res-desc">
          Altı dakikalık güncel diyaloglar, hedef kelime listeleri ve tam metin dökümleriyle düzenli dinleme pratiği sunan podcast serisi.
        </p>
      </div>
      <div class="res-footer">Bölümleri Dinle <span>↗</span></div>
    </a>

    <a href="https://learningenglish.voanews.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="voa learning english voice of america haber dikte dinleme listening sade dil">
      <div>
        <div class="res-header">
          <span class="res-title">VOA Learning English</span>
          <span class="tag-badge tag-audio">Yavaş Haber</span>
        </div>
        <p class="res-desc">
          Normalden daha yavaş tempoyla seslendirilen dünya haberleri; dinleme kavrayışı ve shadowing çalışmaları için ideal kaynak.
        </p>
      </div>
      <div class="res-footer">Haberleri İncele <span>↗</span></div>
    </a>

    <a href="https://www.youtube.com/@engvidRonnie/videos" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="engvid ronnie video youtube konuşma argo slang gramer video ders">
      <div>
        <div class="res-header">
          <span class="res-title">engVid: Ronnie’s Channel</span>
          <span class="tag-badge tag-youtube">Video Ders</span>
        </div>
        <p class="res-desc">
          Günlük konuşma kalıplarını, deyimsel ifadeleri ve kafa karıştıran dilbilgisi ayrıntılarını akıcı bir üslupla anlatan video dersler.
        </p>
      </div>
      <div class="res-footer">Kanala Git <span>↗</span></div>
    </a>

    <a href="https://learnenglish.britishcouncil.org/free-resources" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="british council ielts podcast sınav hazırlık iş ingilizcesi dinleme alıştırma">
      <div>
        <div class="res-header">
          <span class="res-title">British Council Resources</span>
          <span class="tag-badge tag-official">Sınav</span>
        </div>
        <p class="res-desc">
          Temel seviyeden ileri düzeye yapılandırılmış ses kayıtları, IELTS ipuçları ve iş İngilizcesine yönelik ücretsiz alıştırma setleri.
        </p>
      </div>
      <div class="res-footer">Materyalleri Aç <span>↗</span></div>
    </a>

    <a href="https://lingua.com/tr/ingilizce/dikte/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="lingua dikte dictation dinleme listening yazma transkript alıştırma ses seviye test">
      <div>
        <div class="res-header">
          <span class="res-title">Lingua: İngilizce Dikte</span>
          <span class="tag-badge tag-audio">Dikte</span>
        </div>
        <p class="res-desc">
          Farklı seviyelerdeki kayıtları dinleyerek duyduğunu yazıya dökme alıştırmaları; dinleme dikkatini ve yazım doğruluğunu geliştirir.
        </p>
      </div>
      <div class="res-footer">Dikte Çalış <span>↗</span></div>
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
          <span class="res-title">Purdue OWL Writing Lab</span>
          <span class="tag-badge tag-academic">APA / MLA</span>
        </div>
        <p class="res-desc">
          Tez ve makale yazımında argüman kurma, paragraf düzeni ile APA ve MLA kaynak gösterme kuralları için temel başvuru kılavuzu.
        </p>
      </div>
      <div class="res-footer">Kılavuza Git <span>↗</span></div>
    </a>

    <a href="https://www.phrasebank.manchester.ac.uk/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="academic" data-keywords="manchester academic phrasebank akademik kalıplar makale yazımı tez giriş sonuç tartışma literatür">
      <div>
        <div class="res-header">
          <span class="res-title">Academic Phrasebank</span>
          <span class="tag-badge tag-academic">Kalıplar</span>
        </div>
        <p class="res-desc">
          Akademik makalelerin giriş, yöntem, literatür taraması ve tartışma bölümlerinde kullanılan standart ifade kalıpları bankası.
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
          <span class="res-title">Cambridge: Conjunctions</span>
          <span class="tag-badge tag-grammar">Bağlaçlar</span>
        </div>
        <p class="res-desc">
          Zaman bağlaçları, yan tümceler ve metin içi mantıksal geçişlerin doğru kullanımı üzerine Cambridge referans kılavuzu.
        </p>
      </div>
      <div class="res-footer">Kılavuzu Oku <span>↗</span></div>
    </a>

    <a href="https://www.engvid.com/english-resource/verbs-followed-by-gerunds-and-infinitives/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="gerund infinitive engvid fiil yapıları verb structures ing to infinitives">
      <div>
        <div class="res-header">
          <span class="res-title">Gerunds & Infinitives</span>
          <span class="tag-badge tag-grammar">Fiil Yapısı</span>
        </div>
        <p class="res-desc">
          Hangi fiilden sonra "-ing", hangisinden sonra "to" geldiğini net ayrımlarla ve örneklerle gösteren pratik başvuru tablosu.
        </p>
      </div>
      <div class="res-footer">Tabloyu İncele <span>↗</span></div>
    </a>

    <a href="https://www.ef.com/wwen/english-resources/english-grammar/pick-right-quantifier/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="ef quantifiers miktar belirteçleri much many few little sayılabilen isimler">
      <div>
        <div class="res-header">
          <span class="res-title">EF: Quantifiers Rehberi</span>
          <span class="tag-badge tag-grammar">Belirteçler</span>
        </div>
        <p class="res-desc">
          Much/many ve few/little gibi sayılabilen ve sayılamayan isimlerle kullanılan miktar belirteçlerini sade örneklerle açıklar.
        </p>
      </div>
      <div class="res-footer">Rehbere Git <span>↗</span></div>
    </a>

    <a href="https://www.englishclub.com/grammar/determiners-quantifiers.php" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="englishclub determiners quantifiers alıştırma test soruları kurallar">
      <div>
        <div class="res-header">
          <span class="res-title">EnglishClub: Determiners</span>
          <span class="tag-badge tag-grammar">Alıştırma</span>
        </div>
        <p class="res-desc">
          Belirteç sistemini özet kurallar, kısa test soruları ve sık yapılan kullanım hataları üzerinden pekiştiren çalışma sayfası.
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
          <span class="res-title">Test-English: Reading</span>
          <span class="tag-badge tag-reading">Seviye Testi</span>
        </div>
        <p class="res-desc">
          Farklı düzeylerdeki okuma parçaları ve anında dönüt veren testleriyle metin kavrama becerilerini ölçen çalışma portalı.
        </p>
      </div>
      <div class="res-footer">Testi Çöz <span>↗</span></div>
    </a>

    <a href="https://lingua.com/english/reading/wonderful-family/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="reading" data-keywords="lingua reading practice metin okuma parça sorular değerlendirme öykü">
      <div>
        <div class="res-header">
          <span class="res-title">Lingua: Reading Practice</span>
          <span class="tag-badge tag-reading">Metin Okuma</span>
        </div>
        <p class="res-desc">
          Seviyelere göre ayrılmış kısa metinler ve kavrama soruları üzerinden okuma hızını ve anlama yetisini geliştiren kaynak.
        </p>
      </div>
      <div class="res-footer">Metinleri Oku <span>↗</span></div>
    </a>

  </div>
</div>

<!-- İNTERAKTİF DİL & ÇEVİRİ TESTLERİ -->
<section class="quiz-section" id="interaktif-testler">
  <h2 class="category-title" style="border: none; padding-bottom: 0; margin-bottom: 0.35rem;">⚡ İnteraktif Dil & Çeviri Testleri</h2>
  <p class="quiz-section-intro">
    Seviyenizi seçerek <strong>Bağlaç & Eşdizim (Collocation)</strong> bilginizi sınayabilir veya çeviride sık karşılaşılan <strong>İngilizce–Türkçe Çeviri Tuzakları</strong> testini çözebilirsiniz.
  </p>

  <div class="tools-grid">
    <!-- TEST 1: SEVİYELİ BAĞLAÇ & EŞDİZİM TESTİ -->
    <div class="tool-card">
      <div class="tool-header">
        <strong>📘 Seviyeli Bağlaç & Eşdizim Testi</strong>
        <span class="tool-badge" id="activeLevelBadge">B1–B2</span>
      </div>

      <div class="level-tabs" role="tablist" aria-label="Test Seviyesi Seçimi">
        <button type="button" class="level-tab" data-level="a1a2">A1–A2</button>
        <button type="button" class="level-tab active" data-level="b1b2">B1–B2</button>
        <button type="button" class="level-tab" data-level="academic">YDS / İleri</button>
      </div>

      <div class="quiz-box">
        <div class="quiz-top">
          <span id="quizProgress">Soru 1 / 5</span>
          <span id="quizScore">Skor: 0</span>
        </div>
        <p id="quizQuestion" class="quiz-question"></p>
        <div id="quizOptions" class="quiz-options"></div>
        <div id="quizFeedback" class="quiz-feedback" style="display:none;"></div>
        <button type="button" id="nextQuestionBtn" class="quiz-next-btn" style="display:none;">Sonraki Soru →</button>
      </div>
    </div>

    <!-- TEST 2: ÇEVİRİ TUZAKLARI & FALSE FRIENDS -->
    <div class="tool-card">
      <div class="tool-header">
        <strong>🔄 Çeviri Tuzakları & Doğal Karşılıklar</strong>
        <span class="tool-badge">Çeviribilim</span>
      </div>
      <p class="tool-sub">Göründüğü gibi çevrildiğinde anlam kaymasına yol açan ifadelerin bağlama en uygun Türkçe karşılığını seçin.</p>

      <div class="quiz-box">
        <div class="quiz-top">
          <span id="trProgress">Soru 1 / 5</span>
          <span id="trScore">Skor: 0</span>
        </div>
        <p id="trQuestion" class="quiz-question"></p>
        <div id="trOptions" class="quiz-options"></div>
        <div id="trFeedback" class="quiz-feedback" style="display:none;"></div>
        <button type="button" id="trNextBtn" class="quiz-next-btn secondary" style="display:none;">Sonraki Soru →</button>
      </div>
    </div>
  </div>
</section>

<!-- İLETİŞİM & DERS TALEBİ FORMU -->
<div class="resource-contact-section">
  <div class="contact-box">
    <h2 class="category-title" style="border: none; padding-bottom: 0; margin-bottom: 0.45rem;">📬 Yüz Yüze & Online İletişim</h2>
    <p>
      Yüz yüze veya <strong>online İngilizce özel ders</strong> (YDS, YÖKDİL, TOEFL, LGS, konuşma pratiği) ile <strong>Subtitle Edit & SDL Trados Studio</strong> sunumları için form üzerinden ulaşabilirsiniz. Telefonla dönüş isterseniz numaranızı bırakmanız yeterlidir.
    </p>

    <form action="https://formspree.io/f/myewyjgq" method="POST" class="custom-contact-form">
      <div class="form-row">
        <div class="form-group">
          <label for="name">Adınız Soyadınız *</label>
          <input type="text" id="name" name="name" placeholder="Adınız Soyadınız" required />
        </div>

        <div class="form-group">
          <label for="email">E-posta Adresiniz *</label>
          <input type="email" id="email" name="_replyto" placeholder="ornek@email.com" required />
        </div>
      </div>

      <div class="form-row">
        <div class="form-group">
          <label for="program">İlgilendiğiniz Alan</label>
          <select id="program" name="program">
            <option value="YDS / YÖKDİL / TOEFL Özel Ders">YDS / YÖKDİL / TOEFL Özel Ders</option>
            <option value="LGS & Okul İngilizce Takviyesi">LGS & Ortaokul-Lise İngilizce</option>
            <option value="Konuşma & Genel İngilizce">Konuşma & Genel İngilizce</option>
            <option value="Subtitle Edit / SDL Trados Studio Sunumu">Subtitle Edit / SDL Trados Studio Sunumu</option>
            <option value="Diğer / Akademik Danışmanlık">Diğer / Akademik Danışmanlık</option>
          </select>
        </div>

        <div class="form-group">
          <label for="phone">Telefon Numaranız (İsteğe bağlı)</label>
          <input type="tel" id="phone" name="phone" placeholder="05XX XXX XX XX" />
        </div>
      </div>

      <div class="form-group">
        <label for="message">Mesajınız *</label>
        <textarea id="message" name="message" rows="3" placeholder="Hedefiniz, mevcut seviyeniz veya yüz yüze / online tercihiniz..." required></textarea>
      </div>

      <button type="submit" class="submit-btn">Mesajı Gönder ↗</button>
    </form>

    <div class="internal-links-bar">
      <a href="/">← Ana Sayfaya Dön</a>
      <span>•</span>
      <a href="/#ceviribilim-atolye">Subtitle Edit & SDL Trados Studio</a>
      <span>•</span>
      <a href="/#dersler">Özel Ders Bilgileri</a>
    </div>
  </div>
</div>

<!-- ARAMA, FİLTRELEME VE TEST JAVASCRIPT KODU -->
<script>
  document.addEventListener('DOMContentLoaded', function () {
    // 1. KAYNAK ARAMA & FİLTRELEME
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

    // 2. SEVİYELİ BAĞLAÇ & EŞDİZİM TESTİ
    const questionBank = {
      a1a2: [
        {
          q: "I wanted to go for a walk, ______ it started to rain heavily.",
          options: ["because", "but", "so", "or"],
          answer: 1,
          note: "Zıtlık bağlacı: 'but' (ama / fakat), yürüyüş isteği ile yağmur yağması arasındaki karşıtlığı bağlar."
        },
        {
          q: "She always ______ her homework before watching television.",
          options: ["makes", "does", "takes", "puts"],
          answer: 1,
          note: "Temel eşdizim (collocation): İngilizcede 'ödev yapmak' kalıbı 'do homework' fiiliyle kurulur."
        },
        {
          q: "We stayed at home ______ the weather was very cold.",
          options: ["because", "although", "but", "however"],
          answer: 0,
          note: "Sebep bağlacı: 'because' (çünkü), evde kalma nedenini açıklar."
        },
        {
          q: "Please ______ a decision soon so we can book the tickets.",
          options: ["do", "make", "give", "say"],
          answer: 1,
          note: "Temel eşdizim: 'Karar vermek' anlamında 'make a decision' kalıbı kullanılır."
        },
        {
          q: "You should take an umbrella ______ it rains in the afternoon.",
          options: ["in case", "because of", "despite", "unless"],
          answer: 0,
          note: "Tedbir bağlacı: 'in case' (-erse diye / ihtimaline karşı), önlem alma anlamı katar."
        }
      ],
      b1b2: [
        {
          q: "______ the heavy traffic in the city center, we arrived at the conference on time.",
          options: ["Although", "Despite", "However", "Because of"],
          answer: 1,
          note: "Zıtlık edatı: İsim öbeğinden ('the heavy traffic') önce '-e rağmen' anlamında 'Despite' kullanılır."
        },
        {
          q: "The committee decided to ______ the meeting until next Monday due to scheduling conflicts.",
          options: ["call off", "put off", "take over", "bring up"],
          answer: 1,
          note: "Phrasal verb ayrımı: 'put off' ertelemek (postpone), 'call off' ise tamamen iptal etmek demektir."
        },
        {
          q: "Many students find it difficult to ______ a balance between part-time work and university studies.",
          options: ["strike", "hit", "build", "raise"],
          answer: 0,
          note: "Doğal eşdizim (collocation): 'Denge kurmak / sağlamak' için 'strike a balance' kalıbı tercih edilir."
        },
        {
          q: "You won't notice any real progress in your speaking skills ______ you practice consistently.",
          options: ["as long as", "provided that", "unless", "whereas"],
          answer: 2,
          note: "Koşul bağlacı: 'unless' (-medikçe / -mazsa), cümleye olumsuz koşul anlamı verir."
        },
        {
          q: "The new policy is expected to ______ significant changes in how language courses are taught.",
          options: ["bring about", "come across", "give in", "look after"],
          answer: 0,
          note: "Phrasal verb: 'bring about' (yol açmak / meydana getirmek), bir değişimi tetiklemek anlamında kullanılır."
        }
      ],
      academic: [
        {
          q: "______ machine translation has advanced remarkably, human translators remain indispensable for literary nuance.",
          options: ["Albeit", "Notwithstanding", "Inasmuch as", "While"],
          answer: 3,
          note: "Akademik zıtlık bağlacı: Tam bir cümlenin başında '-e rağmen / -iken' anlamında 'While' doğal ve akıcıdır."
        },
        {
          q: "Researchers must ______ close scrutiny to ethical citation practices throughout their manuscripts.",
          options: ["subject", "devote", "exert", "render"],
          answer: 1,
          note: "İleri düzey eşdizim: 'devote attention / scrutiny to' kalıbı bir konuya özenle eğilmek anlamındadır."
        },
        {
          q: "The archival documents were severely damaged; ______, historians managed to reconstruct the timeline.",
          options: ["consequently", "nonetheless", "moreover", "similarly"],
          answer: 1,
          note: "Zıtlık zarfı: 'nonetheless' (buna rağmen / yine de), olumsuz duruma karşın elde edilen başarıyı bağlar."
        },
        {
          q: "Subtitlers frequently have to ______ brevity over literal completeness to respect reading speed limits.",
          options: ["prioritize", "compromise", "alleviate", "substantiate"],
          answer: 0,
          note: "Bağlamsal fiil seçimi: 'prioritize A over B' (A'yı B'ye öncelemek) akademik ve mesleki metinlerde sık kullanılır."
        },
        {
          q: "The findings are largely consistent with earlier studies, ______ a few minor methodological discrepancies.",
          options: ["save for", "owing to", "in light of", "by virtue of"],
          answer: 0,
          note: "İstisna bağlacı: 'save for' (-hariç / dışında), genel uyuma karşın küçük istisnaları belirtir."
        }
      ]
    };

    const levelLabels = {
      a1a2: 'A1–A2',
      b1b2: 'B1–B2',
      academic: 'YDS / İleri'
    };

    let currentLevel = 'b1b2';
    let currentIdx = 0;
    let score = 0;

    const levelTabs = document.querySelectorAll('.level-tab');
    const levelBadge = document.getElementById('activeLevelBadge');
    const qProgress = document.getElementById('quizProgress');
    const qScore = document.getElementById('quizScore');
    const qText = document.getElementById('quizQuestion');
    const qOptions = document.getElementById('quizOptions');
    const qFeedback = document.getElementById('quizFeedback');
    const nextBtn = document.getElementById('nextQuestionBtn');

    function renderQuiz() {
      const list = questionBank[currentLevel];
      const item = list[currentIdx];
      qProgress.textContent = `Soru ${currentIdx + 1} / ${list.length}`;
      qScore.textContent = `Skor: ${score}`;
      qText.textContent = item.q;
      qOptions.innerHTML = '';
      qFeedback.style.display = 'none';
      nextBtn.style.display = 'none';

      item.options.forEach((opt, idx) => {
        const btn = document.createElement('button');
        btn.type = 'button';
        btn.className = 'quiz-opt-btn';
        btn.textContent = `${String.fromCharCode(65 + idx)}) ${opt}`;
        btn.addEventListener('click', () => {
          const allBtns = qOptions.querySelectorAll('.quiz-opt-btn');
          allBtns.forEach(b => b.disabled = true);

          if (idx === item.answer) {
            btn.classList.add('correct');
            score++;
            qScore.textContent = `Skor: ${score}`;
          } else {
            btn.classList.add('wrong');
            allBtns[item.answer].classList.add('correct');
          }

          qFeedback.textContent = item.note;
          qFeedback.style.display = 'block';
          nextBtn.textContent = currentIdx < list.length - 1 ? 'Sonraki Soru →' : 'Testi Yeniden Başlat ↻';
          nextBtn.style.display = 'inline-block';
        });
        qOptions.appendChild(btn);
      });
    }

    levelTabs.forEach(tab => {
      tab.addEventListener('click', () => {
        levelTabs.forEach(t => t.classList.remove('active'));
        tab.classList.add('active');
        currentLevel = tab.getAttribute('data-level');
        levelBadge.textContent = levelLabels[currentLevel];
        currentIdx = 0;
        score = 0;
        renderQuiz();
      });
    });

    nextBtn.addEventListener('click', () => {
      const list = questionBank[currentLevel];
      if (currentIdx < list.length - 1) {
        currentIdx++;
      } else {
        currentIdx = 0;
        score = 0;
      }
      renderQuiz();
    });

    renderQuiz();

    // 3. ÇEVİRİ TUZAKLARI & FALSE FRIENDS TESTİ
    const trQuestions = [
      {
        q: "\"After months of negotiation, the two sides eventually reached an agreement.\" cümlesindeki 'eventually' nasıl çevrilmelidir?",
        options: ["Tesadüfen", "Nihayet / Sonunda", "Muhtemelen", "Aniden"],
        answer: 1,
        note: "False Friend (Sahte Eşdeğer): 'Eventually' Türkçe 'eventüel / tesadüfi' demek değildir; uzun bir sürecin ardından 'nihayet, sonunda' anlamına gelir."
      },
      {
        q: "\"She was very sympathetic when I told her about my academic workload.\" cümlesindeki 'sympathetic' kelimesinin doğru karşılığı nedir?",
        options: ["Çok sevimli ve cana yakındı", "Oldukça anlayışlı ve halden anlardı", "Biraz mesafeliydi", "Çok heyecanlıydı"],
        answer: 1,
        note: "Çeviri Tuzağı: 'Sympathetic' Türkçedeki 'sempatik (sevimli)' anlamında değil, 'anlayışlı, empati kuran, halden anlayan' anlamında kullanılır."
      },
      {
        q: "\"We need to make up for the lost time before the deadline.\" cümlesindeki 'make up for' ifadesinin en doğal çevirisi hangisidir?",
        options: ["Kaybedilen zamanı telafi etmek", "Kaybedilen zamanı uydurmak", "Zamanı yeniden planlamak", "Süreyi uzatmak"],
        answer: 0,
        note: "Phrasal Verb Çevirisi: 'Make up' tek başına 'uydurmak/makyaj yapmak' iken, 'make up for' bir eksiği veya kaybı 'telafi etmek' demektir."
      },
      {
        q: "\"It was a sensible decision to double-check the terminology before submitting the translation.\" cümlesindeki 'sensible' ne anlama gelir?",
        options: ["Hassas / Kırılgan", "Mantıklı / Sağduyulu", "Duygusal", "Aceleci"],
        answer: 1,
        note: "Klasik Çeviri Hatası: 'Sensitive' (hassas/duyarlı) ile 'sensible' (mantıklı/sağduyulu) sık karıştırılır. Burada doğru karşılık 'mantıklı'dır."
      },
      {
        q: "\"Actually, the source text contains an ironic reference to 19th-century literature.\" cümlesinin başındaki 'Actually' bağlama en uygun nasıl aktarılır?",
        options: ["Şu anda / Güncel olarak", "Aslında / Doğrusunu söylemek gerekirse", "Gerçekçi bir biçimde", "Tesadüfen"],
        answer: 1,
        note: "False Friend: 'Actually' (aslında) kelimesi 'güncel' anlamına gelen 'current / topical' ile karıştırılmamalıdır."
      }
    ];

    let trIdx = 0;
    let trScoreVal = 0;

    const trProgress = document.getElementById('trProgress');
    const trScore = document.getElementById('trScore');
    const trQuestion = document.getElementById('trQuestion');
    const trOptions = document.getElementById('trOptions');
    const trFeedback = document.getElementById('trFeedback');
    const trNextBtn = document.getElementById('trNextBtn');

    function renderTrQuiz() {
      const item = trQuestions[trIdx];
      trProgress.textContent = `Soru ${trIdx + 1} / ${trQuestions.length}`;
      trScore.textContent = `Skor: ${trScoreVal}`;
      trQuestion.textContent = item.q;
      trOptions.innerHTML = '';
      trFeedback.style.display = 'none';
      trNextBtn.style.display = 'none';

      item.options.forEach((opt, idx) => {
        const btn = document.createElement('button');
        btn.type = 'button';
        btn.className = 'quiz-opt-btn';
        btn.textContent = `${String.fromCharCode(65 + idx)}) ${opt}`;
        btn.addEventListener('click', () => {
          const allBtns = trOptions.querySelectorAll('.quiz-opt-btn');
          allBtns.forEach(b => b.disabled = true);

          if (idx === item.answer) {
            btn.classList.add('correct');
            trScoreVal++;
            trScore.textContent = `Skor: ${trScoreVal}`;
          } else {
            btn.classList.add('wrong');
            allBtns[item.answer].classList.add('correct');
          }

          trFeedback.textContent = item.note;
          trFeedback.style.display = 'block';
          trNextBtn.textContent = trIdx < trQuestions.length - 1 ? 'Sonraki Soru →' : 'Testi Yeniden Başlat ↻';
          trNextBtn.style.display = 'inline-block';
        });
        trOptions.appendChild(btn);
      });
    }

    trNextBtn.addEventListener('click', () => {
      if (trIdx < trQuestions.length - 1) {
        trIdx++;
      } else {
        trIdx = 0;
        trScoreVal = 0;
      }
      renderTrQuiz();
    });

    renderTrQuiz();
  });
</script>

<!-- SCHEMA.ORG YAPISAL VERİ -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "CollectionPage",
  "name": "İngilizce Çalışma Kaynakları & Testler",
  "description": "YDS, YÖKDİL, TOEFL, LGS hazırlığı ve çeviri çalışmaları için korpus veri tabanları, eşdizim sözlükleri, dikte araçları, seviyeli dil testleri ve iletişim formu.",
  "url": "https://adalienver.site/kaynaklar/",
  "isPartOf": {
    "@type": "WebSite",
    "name": "Enver Adalı — Çeviribilim, Çeviri Teknolojileri & Dil Eğitimi",
    "url": "https://adalienver.site/"
  }
}
</script>
