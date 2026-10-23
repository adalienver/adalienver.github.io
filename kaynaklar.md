---
layout: default
title: İngilizce Öğrenme Materyalleri ve Faydalı Kaynaklar
permalink: /kaynaklar/
---

<style>
  .resource-hero {
    text-align: center;
    margin-bottom: 2rem;
  }
  .resource-hero h1 {
    font-size: 2.1rem;
    color: var(--primary);
    margin-bottom: 0.5rem;
  }
  .resource-hero p {
    color: var(--muted);
    font-size: 1rem;
    max-width: 680px;
    margin: 0 auto;
    line-height: 1.6;
  }

  /* CANLI ARAMA & FİLTRELEME ÇUBUĞU */
  .filter-container {
    background: rgba(255, 255, 255, 0.75);
    border: 1px solid var(--border);
    backdrop-filter: blur(8px);
    border-radius: 12px;
    padding: 1.25rem;
    margin-bottom: 2.5rem;
    box-shadow: 0 4px 15px rgba(21, 50, 91, 0.04);
  }

  .search-input-wrapper {
    position: relative;
    margin-bottom: 1rem;
  }

  .search-input {
    width: 100%;
    padding: 0.75rem 1rem 0.75rem 2.5rem;
    font-size: 0.95rem;
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
    font-size: 1rem;
  }

  .filter-chips {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .chip-btn {
    background: #ffffff;
    border: 1px solid var(--border);
    padding: 0.35rem 0.85rem;
    border-radius: 20px;
    font-size: 0.82rem;
    font-weight: 500;
    color: var(--text);
    cursor: pointer;
    transition: all 0.2s ease;
  }
  .chip-btn:hover {
    border-color: var(--primary);
    color: var(--primary);
  }
  .chip-btn.active {
    background: var(--primary);
    color: #ffffff;
    border-color: var(--primary);
  }

  /* KATEGORİ VE KART DÜZENİ */
  .category-title {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    font-family: 'Lora', serif;
    font-size: 1.3rem;
    color: var(--primary);
    margin-bottom: 1rem;
    border-bottom: 2px solid rgba(0, 0, 0, 0.06);
    padding-bottom: 0.5rem;
  }

  .resource-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(360px, 1fr));
    gap: 1rem;
    margin-bottom: 2.2rem;
  }

  .res-card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: var(--card) !important;
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 1.25rem 1.4rem;
    text-decoration: none;
    color: var(--text) !important;
    transition: all 0.25s ease;
  }

  .res-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(21, 50, 91, 0.08);
    border-color: #b9c7d9;
  }

  .res-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 0.5rem;
    margin-bottom: 0.5rem;
  }

  .res-title {
    font-weight: 600;
    font-size: 1.02rem;
    color: var(--primary);
    line-height: 1.4;
  }

  .res-desc {
    font-size: 0.88rem;
    color: #4a5568;
    line-height: 1.6;
    margin-bottom: 1rem;
  }

  .tag-badge {
    font-size: 0.75rem;
    font-weight: 600;
    padding: 0.25rem 0.65rem;
    border-radius: 999px;
    white-space: nowrap;
    letter-spacing: 0.3px;
  }

  .tag-grammar { background: #e0f2fe; color: #0369a1; }
  .tag-vocab { background: #fef3c7; color: #b45309; }
  .tag-reading { background: #dcfce7; color: #15803d; }
  .tag-audio { background: #f3e8ff; color: #7e22ce; }
  .tag-youtube { background: #fee2e2; color: #b91c1c; }
  .tag-official { background: #ede9fe; color: #6d28d9; }
  .tag-corpus { background: #e0e7ff; color: #3730a3; }
  .tag-context { background: #fae8ff; color: #86198f; }

  .res-footer {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    font-size: 0.82rem;
    font-weight: 600;
    color: var(--accent);
  }

  #no-results-msg {
    display: none;
    text-align: center;
    padding: 2.5rem;
    color: var(--muted);
    font-size: 0.95rem;
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
    Öğrenciler, çevirmen adayları ve dil sınavlarına (YDS, YÖKDİL, TOEFL, IELTS) hazırlananlar için derlenmiş interaktif platformlar, dinleme kanalları, korpus veri tabanları ve dilbilgisi kılavuzları.
  </p>
</div>

<!-- CANLI FİLTRELEME & ARAMA ÇUBUĞU -->
<div class="filter-container">
  <div class="search-input-wrapper">
    <span class="search-icon">🔍</span>
    <input type="text" id="resourceSearch" class="search-input" placeholder="Kaynak adı, konu veya etiket arayın (örn. Korpus, Bağlaç, Dinleme)..." />
  </div>
  <div class="filter-chips">
    <button class="chip-btn active" data-category="all">Tümü</button>
    <button class="chip-btn" data-category="audio">🎧 Dinleme & Video</button>
    <button class="chip-btn" data-category="grammar">📘 Dilbilgisi & Yapı</button>
    <button class="chip-btn" data-category="corpus">🔍 Korpus & Sözlükler</button>
    <button class="chip-btn" data-category="reading">📖 Okuma & Test</button>
  </div>
</div>

<div id="no-results-msg">Aradığınız kritere uygun kaynak bulunamadı.</div>

<!-- 1. DİNLEME, HABER & MULTİMEDYA -->
<div class="category-section" data-section="audio">
  <h2 class="category-title">🎧 Dinleme, Haber & Video Kanalları</h2>
  <div class="resource-grid">

    <a href="https://www.youtube.com/@engvidRonnie/videos" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="engvid ronnie video youtube konuşma argo slang gramer ders">
      <div>
        <div class="res-header">
          <span class="res-title">engVid: Ronnie’s English Channel</span>
          <span class="tag-badge tag-youtube">YouTube Video</span>
        </div>
        <p class="res-desc">
          Doğal konuşma dili, argo (slang), günlük ifadeler ve kafa karıştıran gramer kalıplarını samimi bir üslupla anlatan video ders serisi.
        </p>
      </div>
      <div class="res-footer">Kanala Git ↗</div>
    </a>

    <a href="https://www.bbc.co.uk/learningenglish/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="bbc learning english 6 minute haber dinleme telaffuz">
      <div>
        <div class="res-header">
          <span class="res-title">BBC Learning English</span>
          <span class="tag-badge tag-official">BBC Portal</span>
        </div>
        <p class="res-desc">
          "6 Minute English", haber bültenleri, telaffuz atölyeleri ve güncel olaylar üzerinden İngilizceyi geliştiren referans platformu.
        </p>
      </div>
      <div class="res-footer">Platformu Aç ↗</div>
    </a>

    <a href="https://learningenglish.voanews.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="voa learning english voice of america haber dikte dinleme listening">
      <div>
        <div class="res-header">
          <span class="res-title">VOA Learning English</span>
          <span class="tag-badge tag-audio">Ses & Haber</span>
        </div>
        <p class="res-desc">
          Basitleştirilmiş kelime kadrosu ve net konuşma temposuyla hazırlanmış dünya haberleri; dinleme ve dikte pratikleri için idealdir.
        </p>
      </div>
      <div class="res-footer">Haberleri İncele ↗</div>
    </a>

    <a href="https://learnenglish.britishcouncil.org/free-resources" target="_blank" rel="noopener noreferrer" class="res-card" data-category="audio" data-keywords="british council ielts podcast sınav hazırlık iş ingilizcesi">
      <div>
        <div class="res-header">
          <span class="res-title">British Council: Free Resources</span>
          <span class="tag-badge tag-official">Kurumsal / Sınav</span>
        </div>
        <p class="res-desc">
          IELTS hazırlık ipuçları, seviyelendirilmiş ses kayıtları (podcasts), etkileşimli alıştırmalar ve iş İngilizcesi kaynakları.
        </p>
      </div>
      <div class="res-footer">Materyalleri Aç ↗</div>
    </a>

  </div>
</div>

<!-- 2. DİLBİLGİSİ & YAPISAL ANALİZ -->
<div class="category-section" data-section="grammar">
  <h2 class="category-title">📘 Dilbilgisi & Cümle Mimarisi</h2>
  <div class="resource-grid">

    <a href="https://dictionary.cambridge.org/grammar/british-grammar/conjunctions-time" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="cambridge grammar conjunctions bağlaçlar zaman sentences syntax">
      <div>
        <div class="res-header">
          <span class="res-title">Cambridge Grammar: Conjunctions</span>
          <span class="tag-badge tag-grammar">Bağlaçlar</span>
        </div>
        <p class="res-desc">
          Zaman bağlaçları (when, while, until vb.), yan tümce yapıları ve akademik metinlerde mantıksal geçiş kuralları.
        </p>
      </div>
      <div class="res-footer">Kılavuzu Oku ↗</div>
    </a>

    <a href="https://www.engvid.com/english-resource/verbs-followed-by-gerunds-and-infinitives/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="gerund infinitive engvid fiiller verb structures ing to">
      <div>
        <div class="res-header">
          <span class="res-title">EngVid: Gerunds & Infinitives Table</span>
          <span class="tag-badge tag-grammar">Fiil Yapıları</span>
        </div>
        <p class="res-desc">
          Hangi fiillerin ardından "-ing", hangilerinin ardından "to + verb" geldiğini listeleyen referans tablosu.
        </p>
      </div>
      <div class="res-footer">Tabloyu İncele ↗</div>
    </a>

    <a href="https://www.ef.com/wwen/english-resources/english-grammar/pick-right-quantifier/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="ef quantifiers miktar belirteçleri much many few little sayılabilen">
      <div>
        <div class="res-header">
          <span class="res-title">EF English: Quantifiers</span>
          <span class="tag-badge tag-grammar">Miktar Belirteçleri</span>
        </div>
        <p class="res-desc">
          Much/many, few/little, some/any gibi sayılabilen ve sayılamayan isimlerle kullanılan belirteçlerin kuralları.
        </p>
      </div>
      <div class="res-footer">Rehbere Git ↗</div>
    </a>

    <a href="https://www.englishclub.com/grammar/determiners-quantifiers.php" target="_blank" rel="noopener noreferrer" class="res-card" data-category="grammar" data-keywords="englishclub determiners quantifiers alıştırma test soruları">
      <div>
        <div class="res-header">
          <span class="res-title">EnglishClub: Determiners</span>
          <span class="tag-badge tag-grammar">Referans</span>
        </div>
        <p class="res-desc">
          İngilizce belirteç sistemine dair sade kurallar, test soruları ve sık yapılan hataların analizi.
        </p>
      </div>
      <div class="res-footer">Alıştırmaları Gör ↗</div>
    </a>

  </div>
</div>

<!-- 3. KELİME, KORPUS & ÇEVİRİ SÖZLÜKLERİ -->
<div class="category-section" data-section="corpus">
  <h2 class="category-title">🔍 Kelime Dağarcığı, Korpus & Çeviri Sözlükleri</h2>
  <div class="resource-grid">

    <a href="https://www.english-corpora.org/coca/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="coca corpus american english akademik dilbilim derlem eşdizim frekans">
      <div>
        <div class="res-header">
          <span class="res-title">COCA (Corpus of Contemporary American)</span>
          <span class="tag-badge tag-corpus">Akademik Korpus</span>
        </div>
        <p class="res-desc">
          1 milyardan fazla kelimeden oluşan, sözcük sıklığı ve akademik eşdizimleri incelemek için kapsamlı korpus veri tabanı.
        </p>
      </div>
      <div class="res-footer">Korpusu İncele ↗</div>
    </a>

    <a href="https://sentencedict.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="sentencedict cümle arama örnek cümle bağlam context">
      <div>
        <div class="res-header">
          <span class="res-title">SentenceDict (Örnek Cümle Motoru)</span>
          <span class="tag-badge tag-context">Bağlamsal Kullanım</span>
        </div>
        <p class="res-desc">
          Aradığınız kelimenin gerçek metinler içindeki farklı seviyelerdeki cümle kalıplarını listeleyen arama aracı.
        </p>
      </div>
      <div class="res-footer">Cümle Bul ↗</div>
    </a>

    <a href="https://dictionary.reverso.net/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="reverso context dictionary çeviri paralel metin sözlük">
      <div>
        <div class="res-header">
          <span class="res-title">Reverso Context & Dictionary</span>
          <span class="tag-badge tag-context">Bağlam Çevirisi</span>
        </div>
        <p class="res-desc">
          Kelimeleri ve deyimleri milyonlarca iki dilli paralel metin içerisinde aratarak eşdeğerlerini sunan çevirmen aracı.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç ↗</div>
    </a>

    <a href="https://ozdic.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="ozdic collocations eşdizim sözlük preposition fiil tamlama">
      <div>
        <div class="res-header">
          <span class="res-title">Ozdic Collocations Dictionary</span>
          <span class="tag-badge tag-vocab">Çevirmen Başucu</span>
        </div>
        <p class="res-desc">
          Kelimelerin hangi edat ve sıfatlarla doğal eşleştiğini gösteren başucu eşdizim sözlüğü.
        </p>
      </div>
      <div class="res-footer">Sözlüğü Aç ↗</div>
    </a>

    <a href="https://glosbe.com/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="corpus" data-keywords="glosbe çok dilli bellek translation memory paralel corpus">
      <div>
        <div class="res-header">
          <span class="res-title">Glosbe Çok Dilli Paralel Bellek</span>
          <span class="tag-badge tag-corpus">Paralel Metinler</span>
        </div>
        <p class="res-desc">
          Milyarlarca gerçek çeviri cümlesini bağlamıyla inceleyebileceğiniz zengin paralel korpus sözlüğü.
        </p>
      </div>
      <div class="res-footer">Glosbe'yi Aç ↗</div>
    </a>

  </div>
</div>

<!-- 4. OKUMA PRATİĞİ & TESTLER -->
<div class="category-section" data-section="reading">
  <h2 class="category-title">📖 Okuma Kavrama & Seviye Testleri</h2>
  <div class="resource-grid">

    <a href="https://test-english.com/reading/a1/guess-who-a1-english-reading-test/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="reading" data-keywords="test english reading a1 okuma kavrama seviye sınavı">
      <div>
        <div class="res-header">
          <span class="res-title">Test-English: A1 Reading Test</span>
          <span class="tag-badge tag-reading">Seviye Testi</span>
        </div>
        <p class="res-desc">
          Temel seviye okuma metinleri ve anında puanlama yapan etkileşimli kavrama alıştırmaları.
        </p>
      </div>
      <div class="res-footer">Testi Çöz ↗</div>
    </a>

    <a href="https://lingua.com/english/reading/wonderful-family/" target="_blank" rel="noopener noreferrer" class="res-card" data-category="reading" data-keywords="lingua reading practice metin okuma parça sorular">
      <div>
        <div class="res-header">
          <span class="res-title">Lingua: English Reading Practice</span>
          <span class="tag-badge tag-reading">Metin Okuma</span>
        </div>
        <p class="res-desc">
          Farklı zorluk derecelerinde kısa öyküler, makaleler ve metin değerlendirme soruları.
        </p>
      </div>
      <div class="res-footer">Metinleri Oku ↗</div>
    </a>

  </div>
</div>

<!-- ANINDA FİLTRELEME VE ARAMA JAVASCRIPT KODU -->
<script>
  (function() {
    const searchInput = document.getElementById('resourceSearch');
    const chipBtns = document.querySelectorAll('.chip-btn');
    const cards = document.querySelectorAll('.res-card');
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

        // Başlık altında kart kalmadıysa kategori başlığını gizle
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
