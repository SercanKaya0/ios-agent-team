---
name: bug-triage
description: Bug maddelerinde adımları, beklenen ve gerçekleşen davranışı, ortamı ve eksik bilgiyi çıkarır.
---

# Bug analizi

Madde türü "Bug" ise ya da metin bir hatayı anlatıyorsa (çöküyor, görünmüyor, yanlış gösteriyor):

- `steps`: Hatayı oluşturan adımlar, sırayla. Metinde yoksa boş bırak ve `missing`'e "Tekrar üretme adımları" yaz.
- `expected` / `actual`: Olması gereken ve olan davranış.
- `environment`: Cihaz, iOS sürümü, uygulama sürümü, ortam (Dev/Beta/Prod). Yoksa `missing`'e yaz.
- Ekran görüntüsü ya da video ek dosyalarda varsa "Ekte ekran kaydı var" diye belirt.
