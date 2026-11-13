---
name: ios-task-split
description: Loodos iOS şablonuna (MVVM-R) göre işleri ekran, servis, model, analytics ve test parçalarına ayırır.
---

# iOS iş ayırma

Loodos iOS projeleri MVVM-R şablonuyla yazılır. Yeni bir ekran genelde şu işlere ayrılır:

- **Ekran (ui):** Route, Router, ViewController, ViewModel; boş, yükleniyor ve hata durumları.
- **Servis (network):** Endpoint, istek ve yanıt modeli (`*Response`), DataProvider'a ekleme.
- **Veri (data):** Önbellek, UserDefaults ya da Keychain gerekiyorsa.
- **Mantık (logic):** ViewModel'deki kurallar, doğrulamalar, yönlendirmeler (deeplink dahil).
- **Analytics:** Ekran görüntüleme ve buton event'leri.
- **Test:** ViewModel için en az bir XCTest; kritik akış için UI testi gerekiyorsa ayrı iş.

Erişilebilirlik (VoiceOver etiketleri) ve yerelleştirme metinleri ekran işinin kabul kriterine yazılır.
