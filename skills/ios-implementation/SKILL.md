---
name: ios-implementation
description: Loodos iOS projelerinde bir TODO bölümünü projenin mevcut kalıplarına uyarak uygular ve derler.
---

# iOS uygulama

- Yeni ekran: projedeki en yakın ekranı örnek al; Route, Router, ViewController, ViewModel (ve varsa
  Analytic) dosyalarını aynı klasör düzeniyle ekle. Storyboard/XIB kullanma.
- Servis: projedeki DataProvider / endpoint kalıbını izle; yanıt modelleri `*Response` ile biter.
- Durumlar: boş, yükleniyor ve hata durumlarını projedeki ortak bileşenlerle göster.
- Bool'lar `is` / `has` / `should` ile başlar; `print` bırakma.
- Derleme: `xcodebuild -list` ile şemayı bul, simülatör için Debug derle
  (`-destination 'generic/platform=iOS Simulator'`). Paket çözümü uzun sürebilir; bekle.
- Bitirdiğin her maddeyi kimliğiyle raporla; yarım kalanın nedenini yaz.
