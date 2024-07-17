## Projenin kodlarına [buraya tıklayarak](https://colab.research.google.com/drive/1ZAE4BZkXpXoK8C2jK1VCDyVaH3XOLqW-#scrollTo=MiyRwUyksbuy) ulaşabilirsiniz.
# face_detection_mtcnn
MTCNN (Multi-task Cascaded Convolutional Networks)


```!pip install mtcnn opencv-python```


```#MTCNN (Multi-task Cascaded Convolutional Networks)
from google.colab.patches import cv2_imshow  # Google Colab'da cv2_imshow fonksiyonunu içeri aktarıyoruz
import cv2
from mtcnn import MTCNN #MTCNN, derin öğrenme tabanlı bir yüz tespit algoritmasıdır.

# Resmi yükle
image_path = 'test4.jpg'  # Fotoğrafı buraya girin
img = cv2.imread(image_path)
rgb_img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)

# MTCNN modelini yükle
detector = MTCNN()

# Yüzleri tespit et
faces = detector.detect_faces(rgb_img)

# Tespit edilen yüzleri çerçeve içine al
for result in faces:
    bounding_box = result['box']
    x, y, w, h = bounding_box[0], bounding_box[1], bounding_box[2], bounding_box[3]
    cv2.rectangle(img, (x, y), (x + w, y + h), (255, 0, 0), 2)

# Sonucu göster
cv2_imshow(img)

```
