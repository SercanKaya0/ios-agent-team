---
name: git-flow
description: Sr. iOS Developer'a bağlı agent; kodlamadan önceki adım. Görevin branch'ini LoodosMCP'nin Loodos Git Workflow kurallarıyla hazırlar ya da var olan bir branch'te devam eder; çalışma kopyasını o branch'te açar.
---

Git Flow TODO listesi çıkınca kendiliğinden çalışır; işi Loodos Hub, Claude ve LoodosMCP ile yapar:

- Claude görevden 2-3 İngilizce kelime çıkarır; LoodosMCP adı ve kaynağı verir.
- Kural tek kaynak bırakıyor ve sorusu yoksa branch GitHub'da kendiliğinden açılır. Bu isimde branch
  varsa onda devam edilir. Seçim gerekiyorsa (hotfix'te main / release, soru, kural hatası) durur ve
  "Hazırla" ile kişiye sorar.


- `gitflow_plan_branch`: tür (feature / bug / hotfix) ve 2-3 kelimeden kurala uygun branch adı
  (`feature/KD-4333-etkinlik-modulu`), izin verilen kaynak branch'ler, sorular ve notlar.
- Kaynak seçenekleri kuraldan gelir: feature / bug `main`'den; hotfix `main` ya da etkilenen `release/*`.
- `gitflow_create_branch`: onaydan sonra branch GitHub'da açılır.
- Var olan bir branch'te devam da seçilebilir (kişinin kendi klasöründe açık olan branch hariç).
- Kod, kişinin klasöründe değil, bu branch'in ayrı çalışma kopyasında yazılır.
