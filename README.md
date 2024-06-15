LSTM Model README
Proje Özeti
Bu projede, LSTM (Long Short-Term Memory) modeli kullanılarak Tesla'nın hisse senedi fiyatlarının tahmin edilmesi amaçlanmıştır. 
Proje, geçmiş hisse senedi verilerini kullanarak gelecekteki fiyatları tahmin etmek üzere tasarlanmıştır.

İçindekiler
İş Problemi
Veriyi Anlama
Veriyi Hazırlama
Modelleme
Değerlendirme
Grafikler ve Sonuçlar
Gereksinimler
Kurulum
Kullanım
Sonuç

İş Problemi
Bu projenin amacı, Tesla'nın hisse senedi fiyatlarını geçmiş veriler kullanarak tahmin etmektir. Bu tahminler, yatırımcılara ve analistlere gelecekteki 
fiyat hareketlerini öngörme konusunda yardımcı olabilir.

Veriyi Anlama
Veri seti, Tesla'nın hisse senedi fiyatlarına ait günlük verileri içermektedir. Bu veriler şu sütunları içermektedir:

Date: İlgili işlem gününün tarihi
Open: İlgili işlem gününe ait açılış fiyatı
High: İlgili işlem gününde ulaşılan en yüksek fiyat
Low: İlgili işlem gününde ulaşılan en düşük fiyat
Close: İlgili işlem gününde kapanış fiyatı
Adj Close: Kapanış fiyatının düzeltilmiş hali
Volume: İlgili işlem gününde işlem gören hisse sayısı
Veriyi Hazırlama
Veri işleme adımları şunlardır:

Verinin yüklenmesi ve incelenmesi.
Eksik verilerin kontrol edilmesi ve temizlenmesi.
Verinin ölçeklendirilmesi (0-1 aralığına çekilmesi).
Eğitim ve test setlerine ayrılması.

Modelleme
LSTM modeli, zaman serisi verilerini işlemek için uygun bir derin öğrenme modelidir. Bu projede, Keras kütüphanesi kullanılarak bir LSTM modeli oluşturulmuştur.
Model, geçmiş hisse senedi fiyatlarını kullanarak gelecekteki fiyatları tahmin eder.

Modelin mimarisi:

Girdi katmanı
LSTM katmanı
Dropout katmanı
Tam bağlantılı (Dense) katman
Değerlendirme
Modelin performansı, eğitim ve test veri setlerinde hesaplanan Kök Ortalama Kare Hatası (RMSE) ile değerlendirilmiştir. Ayrıca, eğitim ve doğrulama kayıplarının grafikleri incelenmiştir.

Grafikler ve Sonuçlar
Modelin eğitim sürecinde elde edilen eğitim ve doğrulama kayıpları aşağıdaki gibidir:


Eğitim RMSE: 14.462
Test RMSE: 33.295

Gereksinimler
Projenin çalışması için gerekli kütüphaneler:

numpy
pandas
tensorflow
matplotlib
sklearn
Kurulum

Gerekli kütüphaneleri yüklemek için aşağıdaki komutu kullanabilirsiniz:
pip install numpy pandas tensorflow matplotlib sklearn

Kullanım
Projenin çalıştırılması için aşağıdaki adımları takip edebilirsiniz:

Veri setini TSLA.csv dosyasından yükleyin.
model.py dosyasını çalıştırarak modeli eğitin.
Eğitim tamamlandıktan sonra sonuçları ve grafikleri inceleyin.

Sonuç
Bu projede, LSTM modeli kullanılarak Tesla'nın hisse senedi fiyatlarının tahmin edilmesi sağlanmıştır. Modelin performansı,
eğitim ve test veri setlerinde değerlendirilmiş ve sonuçlar analiz edilmiştir. Bu çalışma, yatırımcılara ve analistlere gelecekteki fiyat hareketlerini öngörmede yardımcı olabilir.

