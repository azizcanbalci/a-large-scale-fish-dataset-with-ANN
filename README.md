# a-large-scale-fish-dataset-with-ANN
 [AKbank Deep Learning Ödevi-a-large-scale-fish-dataset-with-ANN](https://www.kaggle.com/code/azizcanbalc/a-large-scale-fish-dataset-with-ann)

# Balık Türü Sınıflandırma Projesi

Bu proje, derin öğrenme yöntemlerini kullanarak balık türlerini sınıflandırmak amacıyla geliştirilmiştir.

## Kullanılan Kütüphaneler

Gerekli tüm Python kütüphaneleri yüklenmiştir:

- TensorFlow
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Kurulum

```bash
pip install tensorflow pandas numpy matplotlib seaborn '''





Veri Seti Hazırlığı
Kaggle'dan büyük ölçekli bir balık veri seti kullanılıyor. Görüntü dosyalarının yolları ve etiketleri toplanıp bir Pandas DataFrame'e aktarılıyor.

Veri Görselleştirme
Veri setindeki balık türlerinin görselleri görselleştiriliyor ve etiketlerin dağılımı bir çubuk grafikle gösteriliyor.

Görüntülerin İşlenmesi
Görseller yeniden boyutlandırılıyor (225x225) ve normalize ediliyor.

Veri Bölünmesi
Veri seti eğitim, doğrulama ve test setlerine ayrılıyor.

Veri Artırma
Eğitim seti üzerinde görüntülerin dönüş, kaydırma ve yatay çevirme gibi işlemlerle artırma uygulanıyor.

One-Hot Encoding
Etiketler sayısal verilere dönüştürülüyor.

Modelin Tanımlanması
İki gizli katman içeren bir sinir ağı oluşturuluyor. Model, 256 ve 128 nöronlu katmanlar ile oluşturulmuş ve Dropout katmanları ile aşırı öğrenmeyi engelliyor.

Modelin Eğitimi
Model, categorical_crossentropy kaybı ve accuracy metriği ile eğitim alıyor. Eğitim esnasında modelin doğrulama doğruluğu ve kaybı her epoch sonunda raporlanıyor.

Sonuçlar
Modelin doğrulama doğruluğu ilk başlarda %36 iken, 17. epoch sonunda %89 doğruluğa ulaşmış.
