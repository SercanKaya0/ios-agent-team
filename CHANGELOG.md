# Yenilikler

## 0.11.0 · 2026-11-13
- Git Flow eklendi (geliştirmenin ilk adımı): branch LoodosMCP kurallarıyla hazırlanır; tür, isim ve kaynak seçenekleri LoodosMCP'den gelir, onayla GitHub'da açılır. Var olan branch'te devam da seçilebilir.
- iOS Developer, Git Flow'un branch'inde çalışır.
- Jira Publisher en sona alındı: rapor, TODO, biten maddeler ve çelişki cevapları birlikte Jira'ya gider.
- Çelişkiler Hub'da cevaplanır; cevaplanan çelişkiye bağlı bölümlerin kilidi açılır, cevaplar kodlama yönergesine girer.

## 0.10.0 · 2026-11-13
- Geliştirme aşaması başladı: Sr iOS Developer altında iOS Developer agent'ı.
- Bir TODO bölümünü projenin kalıplarına uyarak, görev için açılan ayrı çalışma kopyasında ve branch'te kodlar, derler; bitirdiği maddeleri raporlar. Commit ve push yapmaz.
- Çelişkisi çözülmemiş bölümler geliştirmeye alınmaz. Aynı bölüm Terminal'de Claude Code ile de açılabilir.
- Skill: iOS uygulama.

## 0.9.0 · 2026-11-13
- Jira Publisher eklendi (analiz aşamasının son adımı): Jira Analyst raporu maddeye yorum, TODO listesi bölüm başına alt görev ve Jira'da işaretlenebilir liste olarak gider.
- Tikler yalnız Jira'da atılır; Hub ilerlemeyi Jira'dan okur. Çözülen çelişkiler bağlı ⚠ işaretlerini söndürür.
- Müşteri Jira'sına yazdığı için her gönderim önizleme ve onayla yapılır.

## 0.8.0 · 2026-11-13
- Drive Hub'dan bağlıysa Hub analiz dokümanlarının tam metnini okuyup agent'lara verir; uzun analizler kesilmeden okunur.

## 0.7.0 · 2026-11-13
- Todo Analyst artık plan yapmıyor: analizdeki, seçilen platformu ilgilendiren her cümleyi yorum katmadan bir maddeye çeviriyor.
- Maddeler analizin bölüm başlıklarıyla gruplanır; ekran metinleri birebir, analiz referanslarıyla.
- Çelişkiler / açık sorular (Ç), varsayımlar (V) ve analizde olmayan ekler (B) ayrı bölümlerde; etkilenen maddeler çelişkiye bağlanır.
- Platform Hub'da seçilir (varsayılan iOS); diğer platformların maddeleri alınmaz.
- Skill: Analizden TODO (eski TODO çıkarma ve iOS iş ayırma kalktı).

## 0.6.0 · 2026-11-13
- Takım aşamalara ayrıldı: Sr Business Analyst (Analiz) ve Sr iOS Developer (Geliştirme). iOS Lead kalktı.
- Todo Analyst eklendi: Jira Analyst'in raporunu devralıp iOS için TODO planı çıkarır (işler, kabul kriterleri, büyüklük, bağımlılıklar, açık sorular, devir notu).
- Devir: Jira Analyst "Başlanabilir" derse Todo Analyst kendiliğinden başlar; eksik varsa ekipten onay bekler.
- Skill'ler: TODO çıkarma, iOS iş ayırma.

## 0.5.0 · 2026-11-13
- Link yerine Hub'da yazılan kısa analiz: Jira Analyst bunu analiz dokümanı yerine okur, analizi "var" sayar.

## 0.4.0 · 2026-11-13
- Jira Analyst önce üç soruyu cevaplar: bug mı özellik mi, Figma var mı, analiz var mı.
- Eksik varsa madde sahibine yazılacak hazır yorumu çıkarır (`ask`).
- Analiz dokümanlarını Google Drive MCP ile kendisi okur; Hub'ın ayrı Drive bağlantısı kalktı.

## 0.3.0 · 2026-11-13
- Jira Analyst, Hub'da elle eklenen analiz ve Figma linklerini maddenin parçası sayar.
- Google Drive bağlıysa analiz dokümanlarının içeriğini okuyup kapsamı ve kabul kriterlerini oradan çıkarır.

## 0.2.0 · 2026-11-13
- iOS Lead eklendi.
- Jira Analyst eklendi: görev gelince ilk o çalışır; Jira maddesinin özeti, Figma ve analiz linkleri, bug bilgisi, yorumlar, eksikler ve hazırlık durumu.
- Skill'ler: Jira okuma, link ayıklama, bug analizi, hazırlık kontrolü.

## 0.1.0 · 2026-11-13
- Takım reposu kuruldu; agent'lar adım adım eklenecek.
