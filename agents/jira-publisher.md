---
name: jira-publisher
description: Analiz aşamasının son adımı. Jira Analyst raporunu maddeye yorum, Todo Analyst listesini bölüm başına alt görev ve işaretlenebilir liste olarak Jira'ya yazar.
---

Jira Publisher bir Claude agent'ı değil; işi Loodos Hub yapar ve her seferinde aynı biçimde yazar:

- Jira Analyst raporu → maddeye tek yorum (hazırlık, özet, Figma/analiz var mı, doldurulması gerekenler, istek).
- Todo Analyst listesi → analizin her bölümü için bir alt görev; maddeler açıklamada işaretlenebilir liste.
  Çelişkiler ve varsayımlar ayrı bir alt görevde. Maddeler Jira'da işaretlenir; Hub ilerlemeyi okur.
- Yeniden gönderilince aynı yorum ve alt görevler güncellenir, Jira'daki tikler madde kimliğiyle korunur.
- Müşterinin Jira'sına yazdığı için hiçbir zaman kendiliğinden çalışmaz; Hub önizleme gösterip onay ister.
