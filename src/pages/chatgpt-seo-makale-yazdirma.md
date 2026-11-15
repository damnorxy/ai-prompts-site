---
title: "ChatGPT SEO Makale Promptu: 2000 Kelimelik İçerik Şablonu"
description: "ChatGPT SEO makale promptu ile Google ilk sayfa odaklı, 2000 kelimelik, semantik ve kapsamlı blog içeriklerini adım adım üretin."
pubDate: "2026-11-16"
category: "chatgpt"
---

ChatGPT, varsayılan komutlarla çalıştırıldığında genellikle 500-700 kelimelik yüzeysel özetler üretir ve derinlemesine içerik taleplerini karşılayamaz. Bu kılavuz, semantik SEO metriklerini gözeterek tek bir akışta 2000 kelimelik, taranabilir ve optimize edilmiş içerik üretmenizi sağlayan operasyonel şablonu sunar.

### Ana Prompt Şablonu

```markdown
Rol: Kıdemli SEO İçerik Stratejisti ve Konu Uzmanı (Subject Matter Expert).
Görev: "[Hedef Anahtar Kelime]" odağında, arama niyetini (search intent) %100 karşılayan, derinlemesine, 2000 kelimelik kapsamlı bir SEO makalesi yaz.

Teknik & Biçimsel Kurallar:
1. Uzunluk: Makale kesinlikle minimum 2000 kelime olmalıdır. Her H2 bölümü en az 300-400 kelimelik detaylı alt açıklamalar, örnekler ve uygulanabilir adımlar içermelidir.
2. Yapı: 
   - 1 adet H1 başlığı (Tıklama oranı odaklı, anahtar kelime içeren).
   - En az 5 adet H2 başlığı.
   - Her H2 altında gerekli görülen yerlerde en az 2 adet H3 alt başlığı.
   - 1 adet Sıkça Sorulan Sorular (SSS) bölümü (En az 4 soru-cevap, H2 formatında).
3. Semantik SEO: Aşağıda verilen İkincil ve LSI Anahtar Kelimeleri metin içinde doğal ve bağlamsal olarak geçir.
4. Yazım Tonu: [Ton Belirleyin: örn. Profesyonel, analitik, doğrudan, eğitici]. Gereksiz dolgu kelimelerden ("Sonuç olarak", "Günümüz dünyasında", "Özetle" vb.) kaçın.
5. Veri ve Görselleştirme: İçeriği okunabilir kılmak için en az 1 adet Markdown formatında karşılaştırma tablosu ve maddeli listeler ekle.

Girdi Parametreleri:
- Hedef Anahtar Kelime: [Birincil Kelime]
- İkincil / LSI Kelimeler: [Kelime 1, Kelime 2, Kelime 3, Kelime 4, Kelime 5]
- Hedef Kitle: [Kitle tanımı: örn. E-ticaret yöneticileri, yazılımcılar, yeni başlayanlar]
- Arama Niyeti: [Bilgi Verici / Ticari / Karşılaştırmalı]

Çıktıyı doğrudan makale başlığıyla başlat; giriş veya meta yorum yapma.
```

### Kullanım Örneği

```markdown
Rol: Kıdemli SEO İçerik Stratejisti ve Konu Uzmanı (Subject Matter Expert).
Görev: "ChatGPT SEO makale promptu" odağında, arama niyetini %100 karşılayan, derinlemesine, 2000 kelimelik kapsamlı bir SEO makalesi yaz.

Teknik & Biçimsel Kurallar:
1. Uzunluk: Makale kesinlikle minimum 2000 kelime olmalıdır. Her H2 bölümü en az 300-400 kelimelik detaylı alt açıklamalar, örnekler ve uygulanabilir adımlar içermelidir.
2. Yapı: 
   - 1 adet H1 başlığı.
   - En az 5 adet H2 başlığı.
   - Her H2 altında en az 2 adet H3 alt başlığı.
   - 1 adet Sıkça Sorulan Sorular (SSS) bölümü (4 soru-cevap).
3. Semantik SEO: Aşağıda verilen İkincil ve LSI Anahtar Kelimeleri metin içinde doğal ve bağlamsal olarak geçir.
4. Yazım Tonu: Teknik, doğrudan, eyleme geçirilebilir ve uzman.
5. Veri ve Görselleştirme: En az 1 adet Markdown tablosu ve listeleme kullan.

Girdi Parametreleri:
- Hedef Anahtar Kelime: ChatGPT SEO makale promptu
- İkincil / LSI Kelimeler: yapay zeka içerik üretimi, prompt mühendisliği, semantik SEO, blog yazma komutları, arama motoru optimizasyonu
- Hedef Kitle: SEO uzmanları, blog yazarları ve içerik pazarlamacıları
- Arama Niyeti: Bilgi Verici ve Uygulamalı Rehber

Çıktıyı doğrudan makale başlığıyla başlat; giriş veya meta yorum yapma.
```

### Parametreler / İpuçları

* **Çıktı Kesilmesini Önleme:** LLM modelleri tek seferde 2000 kelime üretirken token sınırına takılabilir. Prompt içine `"Cevabın yarım kalırsa 'DEVAM ET' dediğimde tam olarak kaldığın cümleden devam et"` direktifini ekleyin.
* **Bölümleme Tekniği (Chaining):** 2000 kelime hedefini tam tutturmak için promptu iki aşamalı çalıştırın: Önce sadece detaylı H2/H3 anahat planını (outline) onaylatın, ardından her bir H2 başlığını ayrı ayrı yazdırın.
* **Semantik Yoğunluk:** İkincil kelimeleri listelerken sadece kelime öbeği vermeyin; modelin arama motoru varlıklarını (entities) tanıması için ilgili terimlerin hangi bağlamda kullanılacağını parantez içinde belirtin.

### Sık Yapılan Hatalar

* **Kelime Hedefini Parçalamamak:** Modele yalnızca "2000 kelime yaz" demek yerine alt başlıklara düşen kelime kotalarını (örn. "Her H2 minimum 400 kelime olmalıdır") net olarak belirtmemek metnin kısa kesilmesine yol açar.
* **Gereksiz AI Klişelerini Filtrelememek:** Negatif kısıtlama eklenmediğinde ChatGPT, kelime sayısını doldurmak için "Hızla değişen dijital çağda" gibi anlamsız giriş cümleleriyle içeriğin SEO kalitesini ve bilgi yoğunluğunu (information density) düşürür.
