🚇 Metro Rota Bulucu
Bu proje, bir şehirdeki metro ağı üzerinde en az aktarmalı ve en kısa süreli rotaları bulmayı amaçlayan bir Python uygulamasıdır. Proje, Dijkstra ve BFS (Breadth-First Search) algoritmalarını kullanarak metro güzergâhları arasında farklı ulaşım senaryoları için rota çıkarımı yapar.

🧠 Özellikler
📌 Metro istasyonları ve hatları nesne yönelimli olarak tanımlanır.
🔁 İstasyonlar arası çift yönlü bağlantılar desteklenir.
🧭 En az aktarma sayısı ile hedefe ulaşma rotası (BFS ile).
⏱️ En kısa süreli güzergâh hesaplama (Dijkstra algoritması ile).
🎯 Gerçekçi test senaryoları ile örnek rota analizleri.
🗂️ Dosya Yapısı
bash
Copy
Edit
metro_rota_bulucu/
│
├── metro_rota.py         # Ana Python dosyası (algoritmalar + testler)
└── README.md             # Proje dokümantasyonu (bu dosya)
🛠️ Kurulum ve Çalıştırma
📌 Python 3.7+ sürümünün yüklü olduğundan emin olun.

Bu projeyi klonlayın:
bash
Copy
Edit
git clone https://github.com/kullaniciadi/metro-rota-bulucu.git
cd metro-rota-bulucu
Python dosyasını çalıştırın:
bash
Copy
Edit
python metro_rota.py
🎬 Örnek Çıktılar
Uygulama çalıştırıldığında çeşitli test senaryoları için hem en az aktarmalı hem de en hızlı rotalar şu şekilde görüntülenir:

text
Copy
Edit
AŞTİ'den OSB'ye:
En az aktarmalı rota: AŞTİ -> Kızılay -> Ulus -> Demetevler -> OSB
En hızlı rota (19 dakika): AŞTİ -> Kızılay -> Ulus -> Demetevler -> OSB
🧮 Kullanılan Algoritmalar
BFS (Breadth-First Search): En az aktarmalı rota bulunurken kullanılır. Hat geçiş sayısı en az olan yol önceliklendirilir.
Dijkstra: İstasyonlar arası süre dikkate alınarak toplam süresi en kısa olan rota bulunur.
🧱 Sınıf Yapısı
Istasyon: Her metro durağını temsil eder. Komşular, hat bilgisi, ad gibi bilgileri içerir.
MetroAgi: Tüm ağı ve algoritmaları yönetir. İstasyon ve bağlantı ekleme, rota bulma işlemleri bu sınıf üzerinden yapılır.
🧪 Test Senaryoları
Aşağıdaki gibi test senaryoları sisteme dahil edilmiştir:

AŞTİ -> OSB
Batıkent -> Keçiören
Keçiören -> AŞTİ
Kızılay -> Gar
Sıhhiye -> Demetevler
📌 Geliştirme Fikirleri
🔍 Hat bazlı detaylı görselleştirme.
🌍 Harita desteği ile GUI (Tkinter, PyQt vs).
🧭 Kullanıcıdan başlangıç ve hedef istasyon alma (CLI arayüz).
📈 Trafik yoğunluğunu hesaba katmak (dinamik süreler).
💾 JSON/CSV destekli istasyon verisi alma.
👤 Yazar
Adınız Soyadınız – GitHub Profiliniz

