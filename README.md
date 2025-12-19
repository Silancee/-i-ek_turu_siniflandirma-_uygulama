# cicek_turu_siniflandirma_uygulama
# 🌸 Çiçek Türü Sınıflandırma Projesi

Bu proje, **dijital görüntüleme dersi** kapsamında geliştirilmiş olup, yüklenen bir çiçek fotoğrafının türünü **makine öğrenmesi ve derin öğrenme tabanlı Transfer Learning (CLIP)** yöntemiyle tahmin etmeyi amaçlamaktadır. Sistem, tahmin edilen çiçek türü hakkında **kısa metinsel bilgi** sunar ve isteğe bağlı olarak **Türkçe sesli anlatım** da üretir.

---

## 🎯 Proje Amacı

* Bir çiçek fotoğrafından tür tahmini yapmak
* Klasör veya veri seti gerektirmeden (zero-shot learning)
* Kullanıcıya tahmin sonucu, güven oranı ve açıklayıcı bilgi sunmak
* Mobil cihazlardan erişilebilir bir demo oluşturmak

---

## 🧠 Kullanılan Yöntem

Projede **OpenAI CLIP (Contrastive Language–Image Pretraining)** modeli kullanılmıştır.

CLIP modeli:

* Görsel ve metni aynı vektör uzayında temsil eder
* Önceden eğitilmiş bir modeldir
* Yeni sınıflar eklemek için yeniden eğitime ihtiyaç duymaz (zero-shot learning)

Bu sayede Oxford-102 benzeri bir sistem, **klasörsüz ve eğitim gerektirmeden** oluşturulmuştur.

---

## 🛠️ Kullanılan Teknolojiler

* Python
* PyTorch
* OpenAI CLIP (ViT-B/32)
* Gradio (mobil/web demo arayüzü)
* gTTS (Text-to-Speech)
* Google Colab

---

## 🌼 Desteklenen Çiçek Türleri

Projede aşağıdaki çiçek türleri desteklenmektedir:

Rose, Tulip, Sunflower, Daisy, Lily, Orchid, Lavender, Carnation, Violet, Hyacinth, Jasmine, Peony, Begonia, Hydrangea, Daffodil, Cactus, Lotus, Hibiscus, Magnolia, Camellia, Poppy, Iris, Anemone, Freesia, Chrysanthemum, Geranium, Petunia, Zinnia, Gardenia, Azalea, Foxglove, Clematis, Bougainvillea, Oleander, Wisteria, Morning Glory

Yeni çiçek türleri yalnızca listeye eklenerek sisteme dahil edilebilir.

---

## 📱 Mobil Demo Özelliği

Proje, **Gradio** kullanılarak mobil cihazlardan erişilebilir bir demo hâline getirilmiştir.

Kullanıcı adımları:

1. Telefon veya bilgisayardan demo linkine girilir
2. Galeriden veya kameradan çiçek fotoğrafı yüklenir
3. Sistem tür tahmini yapar
4. Çiçek hakkında bilgi ve sesli anlatım sunulur

---

## 🔊 Sesli Anlatım

Tahmin edilen en yüksek olasılıklı çiçek türü için:

* Türkçe metinsel açıklama
* gTTS kütüphanesi ile oluşturulan sesli anlatım

kullanıcıya sunulmaktadır.

---

## ⚙️ Kurulum ve Çalıştırma (Colab)

```bash
pip install torch torchvision ftfy regex tqdm
pip install git+https://github.com/openai/CLIP.git
pip install gradio gTTS
```

Ardından proje kodu çalıştırılarak Gradio bağlantısı üzerinden demo başlatılır.

---

## 📊 Proje Özellikleri

* Zero-shot çiçek sınıflandırma
* Eğitim ve veri seti gerektirmez
* Top-5 tahmin ve güven oranı gösterimi
* Metinsel ve sesli açıklama
* Mobil uyumlu arayüz

---

## 🎓 Akademik Katkı

Bu proje, dijital görüntü işleme ve derin öğrenme alanlarında:

* Transfer Learning
* Çok modlu (görsel + metin) öğrenme
* Kullanıcı odaklı yapay zekâ uygulamaları

konularını uygulamalı olarak göstermektedir.

---

## 👤 Geliştirici

Bu proje, dijital görüntüleme dersi kapsamında öğrenci projesi olarak geliştirilmiştir.

---

## 📌 Not

Google Colab çalışma ortamı geçici olduğu için, her yeni oturumda gerekli kütüphanelerin yeniden kurulması gerekmektedir.

---

🌸 **Bu proje eğitim amaçlıdır ve akademik çalışmalarda örnek olarak kullanılabilir.**
