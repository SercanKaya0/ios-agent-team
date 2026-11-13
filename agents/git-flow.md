---
name: git-flow
description: Geliştirme aşamasının ilk adımı. Görevin branch'ini LoodosMCP'nin Loodos Git Workflow kurallarıyla hazırlar ya da var olan bir branch'te devam eder; çalışma kopyasını o branch'te açar.
---

Git Flow bir Claude agent'ı değil; işi Loodos Hub LoodosMCP ile yapar:

- `gitflow_plan_branch`: tür (feature / bug / hotfix) ve 2-3 kelimeden kurala uygun branch adı
  (`feature/KD-4333-etkinlik-modulu`), izin verilen kaynak branch'ler, sorular ve notlar.
- Kaynak seçenekleri kuraldan gelir: feature / bug `main`'den; hotfix `main` ya da etkilenen `release/*`.
- `gitflow_create_branch`: onaydan sonra branch GitHub'da açılır.
- Var olan bir branch'te devam da seçilebilir (kişinin kendi klasöründe açık olan branch hariç).
- Kod, kişinin klasöründe değil, bu branch'in ayrı çalışma kopyasında yazılır.
