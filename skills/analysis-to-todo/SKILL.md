---
name: analysis-to-todo
description: Bir analiz dokümanını, seçilen platform için cümle cümle, birebir metinlerle ve analiz referanslarıyla izlenebilir bir TODO listesine çevirir.
---

# Analizden TODO

Örnek (Etkinlik analizi, iOS):

- Bölüm: "1.4.2 Etkinlik Ana Sayfası ve Filtreler"
  - H1 · `1.4.2` · Başlık "Lezzet Dolu Bir Etkinlik Planlayın!".
  - H13 · `1.4.2/13` · Bitiş ≤ başlangıç ise "Bitiş saati, başlangıç saatinden sonra olmalıdır." ve "Uygula" pasif.
  - H14 · `1.4.2/14` · "Kişi Sayısı": 1 veya üzeri tam sayı; aksi halde "Geçerli bir kişi sayısı girin.".
- Bölüm: "1.4.1 Genel"
  - G2 · `1.4.1/2` · Tutar kalemleri client'ta hesaplanmaz; sunucudan gelir. (isInfo)
- Çelişki: Ç6 · `1.4.5/2` · "Firma Adı" analizde opsiyonel, Jira yorumunda zorunlu deniyor. Zorunlu mu?
  → R2 maddesinin `conflicts`'ine "Ç6" eklenir.

Dikkat:

- Bir cümle = bir madde; "ve" ile bağlı iki davranış iki madde.
- Tırnak içindeki metinler noktalamasıyla aynen kalır.
- Listede analizin sırası korunur; madde sırası değiştirilmez.
