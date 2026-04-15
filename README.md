Deepfake Security Analysis & Liveness Detection Bypass

Bu proje, TPS (Thin-Plate Spline) ve FOMM (First Order Motion Model) algoritmaları kullanılarak üretilen deepfake videoların, EAR (Eye Aspect Ratio) tabanlı canlılık tespit sistemlerini atlatma kapasitesini analiz eder.
Öne Çıkan Bulgular
•	Genel Başarı Oranı: Yapılan 68 test sonucunda, derin sahte videoların güvenlik sistemlerini %55.8 oranında başarıyla atlattığı gözlemlenmiştir.
•	En Tehlikeli Model: FOMM modeli, akıcı mimik aktarımı sayesinde belirli senaryolarda %75 başarı oranına ulaşmıştır.
•	Kritik Tespit: AI tarafından üretilen (TPDNE) yüzlerin kusursuz simetrisi, canlılık algoritmalarını yanıltmada daha yüksek performans göstermektedir.
Teknik Altyapı
•	Dil/Çatı: Python, PyTorch.
•	Görüntü İşleme: OpenCV, Dlib (68-nokta landmark tespiti).
•	Canlılık Analizi: EAR algoritması üzerinden göz kırpma takibi.
Proje Yapısı
Proje akışı modüler dört ana birimden oluşur:
1.	fetch/: AI tabanlı yüz fotoğraflarının otomatik toplanması.
2.	batch/: batch_tps.py ve batch_deepfake.py ile seri video üretimi.
3.	test/: Model ve donanım uyumu için tekil kalibrasyon denemeleri.
4.	liveness/: Üretilen videoların EAR algoritması ile güvenlik denetimi.
Gereksinimler ve Kurulum
Projenin kütüphane çakışmalarını önlemek için sanal ortam (venv) kullanılması önerilir. Dizin yollarında hata almamak için Windows üzerinde raw string (r"") kullanımı tercih edilmiştir.
________________________________________
Bu çalışma, biyometrik güvenlik sistemlerinin geliştirilmesi amacıyla hazırlanmış bir akademik araştırma raporudur.

