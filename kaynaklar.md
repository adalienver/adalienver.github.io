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

  .category-title {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    font-family: 'Lora', serif;
    font-size: 1.3rem;
    color: var(--primary);
    margin-bottom: 1rem;
    border-bottom: 2px solid #eef2f6;
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
    background: #ffffff;
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 1.25rem 1.4rem;
    text-decoration: none;
    color: var(--text) !important;
    transition: all 0.25s cubic-bezier(0.16, 1, 0.3, 1);
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
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

  @media (max-width: 640px) {
    .resource-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="resource-hero">
  <h1>İngilizce Öğrenme & Çalışma Kaynakları</h1>
  <p>
    Öğrenciler, çevirmen adayları ve dil sınavlarına (YDS, YÖKDİL, TOEFL, IELTS) hazırlananlar için derlenmiş en nitelikli interaktif platformlar, dinleme kanalları, korpus veri tabanları ve dilbilgisi kılavuzları.
  </p>
</div>

<!-- 1. DİNLEME, HABER & MULTİMEDYA -->
<h2 class="category-title">🎧 Dinleme, Haber & Video Kanalları</h2>
<div class="resource-grid">

  <a href="https://www.youtube.com/@engvidRonnie/videos" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">engVid: Ronnie’s English Channel</span>
        <span class="tag-badge tag-youtube">YouTube Video</span>
      </div>
      <p class="res-desc">
        Doğal konuşma dili, argo (slang), günlük ifadeler ve kafa karıştıran gramer kalıplarını samimi ve akılda kalıcı bir üslupla anlatan popüler video ders serisi.
      </p>
    </div>
    <div class="res-footer">Kanala Git ↗</div>
  </a>

  <a href="https://www.bbc.co.uk/learningenglish/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">BBC Learning English</span>
        <span class="tag-badge tag-official">BBC Portal</span>
      </div>
      <p class="res-desc">
        "6 Minute English", haber bültenleri, telaffuz atölyeleri ve güncel olaylar üzerinden İngilizceyi geliştiren küresel referans platformu.
      </p>
    </div>
    <div class="res-footer">Platformu Aç ↗</div>
  </a>

  <a href="https://learningenglish.voanews.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">VOA Learning English (Voice of America)</span>
        <span class="tag-badge tag-audio">Ses & Haber</span>
      </div>
      <p class="res-desc">
        Basitleştirilmiş kelime kadrosu ve anlaşılır, net konuşma temposuyla hazırlanmış dünya haberleri; dinleme ve dikte pratikleri için idealdir.
      </p>
    </div>
    <div class="res-footer">Haberleri İncele ↗</div>
  </a>

  <a href="https://learnenglish.britishcouncil.org/free-resources" target="_blank" rel="noopener noreferrer" class="res-card">
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

<!-- 2. DİLBİLGİSİ & YAPISAL ANALİZ -->
<h2 class="category-title">📘 Dilbilgisi & Cümle Mimarisi</h2>
<div class="resource-grid">

  <a href="https://dictionary.cambridge.org/grammar/british-grammar/conjunctions-time" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Cambridge Grammar: Conjunctions of Time</span>
        <span class="tag-badge tag-grammar">Bağlaçlar</span>
      </div>
      <p class="res-desc">
        Zaman bağlaçları (when, while, as soon as, until vb.), yan tümce yapıları ve akademik metinlerde mantıksal geçiş kuralları.
      </p>
    </div>
    <div class="res-footer">Kılavuzu Oku ↗</div>
  </a>

  <a href="https://www.engvid.com/english-resource/verbs-followed-by-gerunds-and-infinitives/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">EngVid: Gerunds & Infinitives Table</span>
        <span class="tag-badge tag-grammar">Fiil Yapıları</span>
      </div>
      <p class="res-desc">
        Hangi fiillerin ardından "-ing", hangilerinin ardından "to + verb" geldiğini örnek cümlelerle özetleyen pratik referans tablosu.
      </p>
    </div>
    <div class="res-footer">Tabloyu İncele ↗</div>
  </a>

  <a href="https://www.ef.com/wwen/english-resources/english-grammar/pick-right-quantifier/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">EF English: Pick the Right Quantifier</span>
        <span class="tag-badge tag-grammar">Miktar Belirteçleri</span>
      </div>
      <p class="res-desc">
        Much/many, few/little, some/any gibi sayılabilen ve sayılamayan isimlerle kullanılan belirteçlerin doğru kullanım prensipleri.
      </p>
    </div>
    <div class="res-footer">Rehbere Git ↗</div>
  </a>

  <a href="https://www.englishclub.com/grammar/determiners-quantifiers.php" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">EnglishClub: Determiners & Quantifiers</span>
        <span class="tag-badge tag-grammar">Referans</span>
      </div>
      <p class="res-desc">
        İngilizce belirteç sistemine dair sade kurallar, test soruları ve sık yapılan hataların analizi.
      </p>
    </div>
    <div class="res-footer">Alıştırmaları Gör ↗</div>
  </a>

</div>

<!-- 3. KELİME, DEYİM, KORPUS & ÇEVİRİ SÖZLÜKLERİ -->
<h2 class="category-title">🔍 Kelime Dağarcığı, Korpus & Çeviri Sözlükleri</h2>
<div class="resource-grid">

  <a href="https://www.english-corpora.org/coca/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">COCA (Corpus of Contemporary American English)</span>
        <span class="tag-badge tag-corpus">Akademik Korpus</span>
      </div>
      <p class="res-desc">
        1 milyardan fazla kelimeden oluşan, sözcük sıklığı (frequency), türsel dağılım ve akademik metin eşdizimlerini incelemek için en güçlü dilbilimsel korpus veri tabanı.
      </p>
    </div>
    <div class="res-footer">Korpusu İncele ↗</div>
  </a>

  <a href="https://sentencedict.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">SentenceDict (Örnek Cümle Motoru)</span>
        <span class="tag-badge tag-context">Bağlamsal Kullanım</span>
      </div>
      <p class="res-desc">
        Aradığınız herhangi bir İngilizce kelimenin gerçek metinler içindeki farklı seviyelerdeki kullanım biçimlerini ve cümle kalıplarını listeleyen pratik arama aracı.
      </p>
    </div>
    <div class="res-footer">Cümle Bul ↗</div>
  </a>

  <a href="https://dictionary.reverso.net/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Reverso Context & Dictionary</span>
        <span class="tag-badge tag-context">Bağlam Çevirisi</span>
      </div>
      <p class="res-desc">
        Kelimeleri ve deyimleri milyonlarca iki dilli gerçek paralel metin içerisinde aratarak en doğal eşdeğerlerini ve kullanım bağlamlarını sunan çevirmen aracı.
      </p>
    </div>
    <div class="res-footer">Sözlüğü Aç ↗</div>
  </a>

  <a href="https://ozdic.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Ozdic Collocations Dictionary</span>
        <span class="tag-badge tag-vocab">Çevirmen Başucu</span>
      </div>
      <p class="res-desc">
        Kelimelerin ana dili İngilizce olanlar tarafından hangi edat ve sıfatlarla doğal şekilde eşleştiğini (make a decision vs do a decision) gösteren vazgeçilmez eşdizim sözlüğü.
      </p>
    </div>
    <div class="res-footer">Sözlüğü Aç ↗</div>
  </a>

  <a href="https://www.vocabulary.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Vocabulary.com</span>
        <span class="tag-badge tag-vocab">İleri Düzey Kelime</span>
      </div>
      <p class="res-desc">
        Kelimeleri ezberletmek yerine bağlam içi anlamlarını öğreten, akıllı alıştırma döngülerine sahip akademik kelime öğrenme motoru.
      </p>
    </div>
    <div class="res-footer">Kelime Çalış ↗</div>
  </a>

  <a href="https://glosbe.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Glosbe Çok Dilli Paralel Bellek</span>
        <span class="tag-badge tag-corpus">Paralel Metinler</span>
      </div>
      <p class="res-desc">
        Milyarlarca gerçek çeviri cümlesini bağlamıyla inceleyebileceğiniz, terim ve kalıp çevirilerinde çevirmenler ve araştırmacılar için zengin paralel korpus sözlüğü.
      </p>
    </div>
    <div class="res-footer">Glosbe'yi Aç ↗</div>
  </a>

  <a href="https://www.thefreedictionary.com/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">The Free Dictionary (Farlex)</span>
        <span class="tag-badge tag-vocab">Kapsamlı Sözlük</span>
      </div>
      <p class="res-desc">
        Genel İngilizce tanımlarının yanı sıra tıp, hukuk, finans ve bilişim gibi özel alan terimlerini, deyimleri ve kısaltmaları tek çatı altında toplayan devasa referans portalı.
      </p>
    </div>
    <div class="res-footer">Sözlüğü Aç ↗</div>
  </a>

  <a href="https://www.eslcafe.com/resources/idioms" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Dave's ESL Cafe: Idioms Archive</span>
        <span class="tag-badge tag-vocab">Deyimler & Kalıplar</span>
      </div>
      <p class="res-desc">
        Günlük dilde ve metinlerde sıkça karşılaşılan İngilizce deyimleri, gerçek hayattan örnek cümlelerle ve sade açıklamalarla kategorilendiren zengin deyim arşivi.
      </p>
    </div>
    <div class="res-footer">Deyimleri İncele ↗</div>
  </a>

</div>

<!-- 4. OKUMA PRATİĞİ & SEVİYE TESTLERİ -->
<h2 class="category-title">📖 Okuma Kavrama & Seviye Testleri</h2>
<div class="resource-grid">

  <a href="https://test-english.com/reading/a1/guess-who-a1-english-reading-test/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Test-English: A1 Reading Test</span>
        <span class="tag-badge tag-reading">Seviye Testi</span>
      </div>
      <p class="res-desc">
        Temel seviye (A1) okuma metinleri, ipuçları ve anında puanlama yapan etkileşimli kavrama soruları.
      </p>
    </div>
    <div class="res-footer">Testi Çöz ↗</div>
  </a>

  <a href="https://lingua.com/english/reading/wonderful-family/" target="_blank" rel="noopener noreferrer" class="res-card">
    <div>
      <div class="res-header">
        <span class="res-title">Lingua: English Reading Practice</span>
        <span class="tag-badge tag-reading">Metin Okuma</span>
      </div>
      <p class="res-desc">
        Farklı zorluk derecelerinde kısa öyküler, makaleler ve metin altı değerlendirme soruları.
      </p>
    </div>
    <div class="res-footer">Metinleri Oku ↗</div>
  </a>

</div>
