# iOS Agent Team

Loodos Hub'ın **Agent Takımları** sayfasındaki hazır takım. Hub bu repoyu okur, takımı gösterir,
kurar ve repo güncellenince herkesin takımını yeniler. Repoyu okuyabilen kişiler sayfayı görür;
yazma yetkisi olanlar takımı Hub'dan düzenleyebilir.

## Yapı

```
team.json                 Takım: ad, sürüm, Lead'ler ve agent'lar (çalışma sırasıyla)
agents/<id>.md            Her Lead ve agent: Claude Code subagent dosyası
skills/<id>/SKILL.md      Her skill: Claude Code skill dosyası
CHANGELOG.md              Sürüm notları (Hub'da güncelleme bildiriminde görünür)
```

## team.json

```json
{
  "name": "iOS Team",
  "version": "0.2.0",
  "summary": "Loodos iOS ekibinin Claude agent takımı.",
  "members": [
    { "id": "ios-lead", "kind": "lead", "title": "iOS Lead", "role": "Lead · iOS",
      "hue": 262, "face": 0, "tools": ["read", "jira"], "skills": ["plan"] },
    { "id": "design-analyst", "kind": "agent", "lead": "ios-lead", "title": "Design Analyst", "role": "Sr · Tasarım",
      "hue": 160, "face": 1, "tools": ["figma", "read"], "skills": ["figma-tokens"] }
  ]
}
```

- `members` sırası çalışma sırasıdır: bir Lead'in agent'ları listede göründükleri sırayla çalışır.
- `kind`: `lead` ya da `agent`. Agent'ın `lead`'i bağlı olduğu Lead'in `id`'si.
- `hue` (0–359) kartın rengi, `face` (0–7) Hub'daki resmi.
- `tools`: `figma`, `jira`, `drive` (Google Drive), `loodos-mcp`, `xcode` (MCP'ler); agent sadece adı geçen MCP'lerin okuma araçlarını kullanabilir · `read`, `write`, `bash`, `web` (yerleşik).
- Lead'ler aşamadır (Analiz → Geliştirme); görev Lead sırasıyla ilerler.
- `after: "<agent id>"`: Bu agent o agent'ın raporunu devralır ve ondan sonra çalışır.
- `autoWhen: "ready"`: Önceki rapor "Başlanabilir" ise kendiliğinden başlar; değilse Hub'da onay bekler (`always` ise her zaman).
- `runsOn: "task": Hub'da göreve bir Jira maddesi eklenince bu agent kendiliğinden çalışır.
- `output`: Agent'ın rapor biçimi; Hub bu biçimi tanır ve raporu kart olarak gösterir (`jira-analysis`, `todo-plan`).
- Agent dosyasında `model:` (ör. `sonnet`) agent'ın hangi modelle çalışacağını söyler.
- Takımda bir şey değişince `version`'ı artır ve `CHANGELOG.md`'ye yaz; Hub yeni sürümü kurar.

## agents/&lt;id&gt;.md

```markdown
---
name: design-analyst
description: Figma URL'inden tasarım şablonunu çıkarır; ekranlar, font, renk ve boşluklar.
---

Sen Loodos iOS ekibinin Design Analyst'isin. …
```

`description` Hub'da "Ne yapar?" olarak görünür; gövde agent'ın talimatıdır.

## skills/&lt;id&gt;/SKILL.md

```markdown
---
name: figma-tokens
description: Renk, font, spacing ve radius listesini çıkarır.
---

# Tasarım token'ları

…
```

İlk `#` başlığı Hub'da skill'in adı olarak görünür.
