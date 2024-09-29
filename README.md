## Projenin kodlarına [buraya tıklayarak](https://colab.research.google.com/drive/1ZAE4BZkXpXoK8C2jK1VCDyVaH3XOLqW-#scrollTo=MiyRwUyksbuy) ulaşabilirsiniz.
# MTCNN ile Yüz Tespiti ve Bulanıklaştırma Projesi

## Açıklama
Bu proje, MTCNN (Multi-task Cascaded Convolutional Networks) kullanarak resimlerdeki yüzleri tespit eden ve ardından tespit edilen yüzleri bulanıklaştıran bir Python uygulamasıdır. Uygulama, gizlilik gerektiren durumlarda yüzleri maskelemek için idealdir. Derin öğrenme tabanlı bu algoritma, çeşitli açılardan ve koşullarda yüzleri daha hassas bir şekilde tespit etme yeteneğine sahiptir.

## Kullanılan Teknolojiler

### İstemci
- **Python**: Proje, Python programlama dili kullanılarak geliştirilmiştir.
- **OpenCV**: Görüntü işleme ve analiz işlemleri için kullanılan popüler bir kütüphane.
- **MTCNN**: Derin öğrenme tabanlı bir yüz tespit algoritması. Yüzleri tespit etme konusunda yüksek doğruluk sağlar.
- **Google Colab**: Proje, bulut tabanlı bir ortamda çalıştırıldığı için kullanıcılar için erişim kolaylığı sağlar.

### Sunucu
- **Yerel Sunucu**: Proje, istemci tarafında çalıştırıldığından, herhangi bir sunucu yapılandırması gerektirmemektedir. Google Colab, kullanıcının yerel makinesinde kurulum yapmadan projeyi çalıştırmasına olanak tanır.


## Kurulum
Projeyi çalıştırmak için aşağıdaki adımları izleyin:

1. **Google Colab'a Giriş**: Google hesabınızla [Google Colab](https://colab.research.google.com/) platformuna gidin.
2. **Yeni Bir Notebook Oluşturun**: "New Notebook" seçeneğine tıklayarak yeni bir çalışma alanı oluşturun.
3. **Gerekli Kütüphaneleri Yükleme**:
   Aşağıdaki kodu çalıştırarak gerekli kütüphaneleri yükleyin:
   ```python
   !pip install mtcnn opencv-python
4. **Resim Dosyasını Yükleme**: test4.jpg adında bir resim dosyasını Colab ortamınıza yükleyin. Alternatif olarak, kendi resim dosyanızın yolunu image_path değişkenine atayabilirsiniz.

## Kullanım
Yüz tespiti ve blurlama işlemini gerçekleştirmek için kodu çalıştırın.
