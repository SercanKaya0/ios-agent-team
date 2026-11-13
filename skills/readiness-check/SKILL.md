---
name: readiness-check
description: İşe başlamak için gerekenlerin (tasarım, analiz, API, kabul kriteri) hazır olup olmadığına karar verir.
---

# Hazırlık kontrolü

İşe başlamadan önce şunlara bak:

1. Tasarım: Ekran değişikliği varsa Figma linki var mı?
2. Analiz: Davranış metinde ya da bir analiz dokümanında anlatılmış mı?
3. API: Servis gerekiyorsa endpoint ya da API dokümanı belli mi?
4. Kabul kriterleri: Ne zaman "bitti" sayılacağı belli mi?

- Hepsi tamamsa `ready`.
- Biri eksik ama iş başlayabiliyorsa `partial`.
- Ne yapılacağı anlaşılmıyorsa ya da kritik bir parça yoksa `blocked`.
