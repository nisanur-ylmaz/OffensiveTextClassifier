1. Projenin Amacı
Bu projenin amacı, sosyal medya gibi platformlardaki metinleri analiz ederek saldırgan dili otomatik olarak tespit etmek ve saldırgan ifadelerin türlerini sınıflandırmaktır. Proje iki aşamalı bir sınıflandırma süreci izlemektedir: İlk aşamada cümle saldırgan mı değil mi belirlenir; ikinci aşamada ise saldırgan cümleler 'INSULT', 'SEXIST', 'RACIST', 'PROFANITY' gibi türlere ayrılır.
•	INSULT (Hakaret): Kişiye veya gruba yönelik küçük düşürücü, kırıcı, aşağılayıcı ifadeler içerir.
•	SEXIST (Cinsiyetçi): Kadınlara veya erkeklere yönelik cinsiyet temelli ayrımcılık, aşağılayıcı ya da önyargılı söylemler.
•	RACIST (Irkçı): Etnik köken, din veya milliyet temelinde ayrımcılık yapan ya da nefret içeren ifadeler.
•	PROFANITY (Küfürlü): Argo, müstehcen veya küfürlü dil kullanan ifadeler.
•	OTHER (Diğer): Saldırgan olmayan ya da belirli bir kategoriye (hakaret, cinsiyetçilik, ırkçılık, küfür) tam olarak uymayan saldırgan ifadeleri kapsamak için kullanılır

2. Proje Altyapısı ve Kullanılan Donanım
• Programlama Dili: Python
• Geliştirme Ortamı: Jupyter Notebook (.ipynb)
• Derin Öğrenme Kütüphaneleri: Transformers, Torch, Sklearn
• Model: BERTurk (dbmdz/bert-base-turkish-cased)
• Donanım: 16 GB RAM, NVIDIA RTX GPU-3050 
• İşletim Sistemi: Windows 11
3. Test Sonuçları
Proje iki farklı sınıflandırma görevi üzerinden değerlendirilmiştir:
• Binary Sınıflandırma (Saldırgan vs. Değil)
• Multi-Class Sınıflandırma (Saldırganlık Türü)

Test metrikleri:
• Accuracy (Doğruluk): %91.24
• Precision (Kesinlik): %90.7
• Recall (Duyarlılık): %89.3
• F1-Score: %90.0

Confusion Matrix ve Classification Report çıktıları model eğitim sürecinde alınmış ve incelenmiştir.
4. Gerekli Kütüphaneler ve Çalıştırma Adımları
Aşağıdaki komutlar kullanılarak gerekli kütüphaneler yüklenmelidir:
!pip install transformers datasets accelerate scikit-learn

Çalıştırmak için:
1. Jupyter Notebook ya da Python dosyasını açın.
2. Kodun başında veri yolunu kendi bilgisayarınıza göre güncelleyin.
3. 'Run All' veya hücre hücre çalıştırarak modeli eğitin ve test edin.
4. Eğitim sonrası kullanıcıdan alınan cümleler interaktif olarak analiz edilebilir.
