---
name: link-finder
description: Metindeki linkleri türüne göre ayırır: Figma, analiz dokümanı, Confluence, API dokümanı ve diğerleri.
---

# Link ayıklama

Hub linkleri bulup türünü tahmin eder (`links`); sen her linkin metinde ne için verildiğini yaz.

- `figma.com/file`, `figma.com/design`, `figma.com/proto`: tasarım. `node-id` varsa belirli bir ekran ya da bileşendir.
- `docs.google.com`, `drive.google.com`, `sharepoint.com`, `onedrive`: analiz ya da doküman.
- `atlassian.net/wiki`, `confluence`: Confluence sayfası, çoğunlukla analiz.
- `swagger`, `postman`, `/api-docs`, `openapi`: API dokümanı.
- `apps.apple.com`, `play.google.com`, `testflight`: mağaza ya da test linki; `docs`'a `other` olarak yaz.
- Aynı link birden fazla geçiyorsa bir kez yaz.
