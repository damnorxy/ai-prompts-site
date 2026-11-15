---
title: "Claude Kod Refaktör Etme Promptu: Karmaşık Kodları Temizleme Rehberi"
description: "Claude 3.5 Sonnet ile spagetti kodları temizleyin ve modernize edin. İşte en etkili Claude kod refaktör etme promptu ve kullanım rehberi."
pubDate: "2026-11-16"
category: "coding"
---

Geliştirme süreçlerinde biriken teknik borçlar ve spagetti kodlar, projelerin bakımını zorlaştırarak sistem kararlılığını tehdit eder. Bu rehberdeki **Claude kod refaktör etme promptu**, Claude 3.5 Sonnet'in gelişmiş mantıksal analiz yeteneğini kullanarak mevcut işlevselliği bozmadan kod tabanınızı Clean Code ve SOLID standartlarına dönüştürür.

### Ana Prompt Şablonu

```markdown
Sen Kıdemli bir Yazılım Mimarı ve Clean Code uzmanısın. Görevin, sana iletilen karmaşık kodu incelemek ve işlevselliği birebir koruyarak refaktör etmektir.

Analiz Edilecek Kod Bilgileri:
- Programlama Dili / Framework: [DİL / ÇERÇEVE ADI]
- Hedeflenen Mimari Standartlar: [SOLID / DRY / KISS / Temiz Mimari vb.]
- Öncelikli Odak: [Okunabilirlik / Bellek Optimizasyonu / Hata Yönetimi / Modülerlik]

Aşağıdaki kurallara kesinlikle uy:
1. Mevcut girdileri ve çıktıları bozma (Breaking change yaratma).
2. Spagetti yapıları, derin iç içe geçmiş (nested) blokları 'Early Return' deseniyle sadeleştir.
3. Tip güvenliğini artır (type safety) ve anlamlı değişken/fonksiyon adlandırmaları kullan.
4. Refaktör edilmiş kodun hemen altına yapılan mimari değişiklikleri ve kazanımları madde madde özetle.
5. Değişikliğin mantığını doğrulamak için birim test senaryoları (Unit Test) ekle.

Refaktör Edilecek Kod:
```[DİL ADI]
[KODU BURAYA YAPIŞTIRIN]
```
```

### Kullanım Örneği

```markdown
Sen Kıdemli bir Yazılım Mimarı ve Clean Code uzmanısın. Görevin, sana iletilen karmaşık kodu incelemek ve işlevselliği birebir koruyarak refaktör etmektir.

Analiz Edilecek Kod Bilgileri:
- Programlama Dili / Framework: JavaScript (Node.js)
- Hedeflenen Mimari Standartlar: SOLID (Özellikle Single Responsibility) ve Clean Code
- Öncelikli Odak: Okunabilirlik ve Hata Yönetimi

Aşağıdaki kurallara kesinlikle uy:
1. Mevcut girdileri ve çıktıları bozma (Breaking change yaratma).
2. Spagetti yapıları, derin iç içe geçmiş (nested) blokları 'Early Return' deseniyle sadeleştir.
3. Tip güvenliğini artır (type safety) ve anlamlı değişken/fonksiyon adlandırmaları kullan.
4. Refaktör edilmiş kodun hemen altına yapılan mimari değişiklikleri ve kazanımları madde madde özetle.
5. Değişikliğin mantığını doğrulamak için birim test senaryoları (Unit Test) ekle.

Refaktör Edilecek Kod:
```javascript
function processData(users) {
  let res = [];
  if (users && users.length > 0) {
    for (let i = 0; i < users.length; i++) {
      if (users[i].active == true) {
        if (users[i].age >= 18) {
          let fullName = users[i].firstName + ' ' + users[i].lastName;
          res.push({ id: users[i].id, name: fullName });
        }
      }
    }
    return res;
  } else {
    return [];
  }
}
```
```

### Parametreler / İpuçları

1. **Bağlamı (Context) Net Tanımlayın:** Sadece fonksiyonu vermek yerine, kodun bağımlı olduğu kütüphaneleri, çalışma zamanı sürümünü (örn. Node 20, Python 3.12) prompt içine ekleyerek modelin güncel API sentakslarını kullanmasını sağlayın.
2. **Kapsam Daraltma Yapın:** Claude 3.5 Sonnet'e tek seferde 1000 satırlık devasa dosyalar vermek yerine, kodu mantıksal modüllere bölerek (fonksiyon veya sınıf bazında) parça parça refaktör ettirin.
3. **Diff Çıktısı İsteyin:** Büyük kod tabanlarında yapılan değişiklikleri doğrudan görebilmek için prompt sonuna *"Değişiklikleri Git diff formatında göster"* parametresini ekleyin.

### Sık Yapılan Hatalar

* **Aynı Anda Hem Refaktör Hem Yeni Özellik İstemek:** Kodu temizlerken araya yeni işlevsellik talepleri sıkıştırmak, modelin regresyon testlerini ihlal etmesine ve mevcut mantığı kaybetmesine yol açar.
* **Girdi/Çıktı Kısıtlarını Belirtmemek:** API sözleşmesini (contract) modele açıkça bildirmemek, Claude'un veri dönüş yapısını (örn. camelCase yerine snake_case kullanımı gibi) istemeden değiştirmesine neden olabilir.
