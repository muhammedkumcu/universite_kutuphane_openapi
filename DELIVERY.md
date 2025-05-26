
# OpenAPI Tasarımı Ödevi Teslim Raporu

## 👤 Öğrenci Bilgileri
- **Ad Soyad**: Muhammed Kumcu
- **Öğrenci Numarası**: 170422008

---

## 📂 OpenAPI YAML Dosyası

- **openapi.yaml** dosyasını projenizin GitHub reposuna yükledim. Swagger Editor üzerinde test ederek hatasız hale getirdim.

### 🔗 GitHub Repo Linki
[https://github.com/muhammedkumcu/universite_kutuphane_openapi](https://github.com/muhammedkumcu/universite_kutuphane_openapi)

---

## 📝 API Açıklaması

Bu API, üniversitenin çevrim içi kütüphane sistemi için tasarlanmıştır ve üç ana varlık üzerinden CRUD işlemleri sağlamaktadır:

- **Varlıklar (entities)**:  
  - **books**: Kitap bilgilerini yönetir.  
  - **students**: Öğrenci bilgilerini yönetir.  
  - **loans**: Kitap ödünç alma ve iade işlemlerini yönetir.

- **CRUD İşlemleri**:  
  - `GET /books`, `POST /books`, `PUT /books/{id}`, `DELETE /books/{id}`, `GET /books/{id}` gibi endpoint’ler kitaplar için.  
  - Benzer şekilde students ve loans endpoint’leri de aynı CRUD yapısına uygun şekilde tasarlanmıştır.

- **components/schemas**: Tüm veri modelleri (`Book`, `Student`, `Loan`) bu bölümde detaylıca tanımlandı.  
- **parameters**: Path ve query parametreleri (`id`, `page`, `size`) burada tanımlı.  
- **responses**: Hata durumları (`400`, `404`, `500`) ve başarılı cevaplar burada açıklandı.  
- **Sayfalama**: `GET /books` endpoint’inde `page` ve `size` parametreleriyle uygulandı.

- **Ek Açıklamalar**: API key tabanlı basit bir `securitySchemes` örneği de eklendi.

---

## 📌 Ek Açıklamalar

Bu ödev, OpenAPI 3.0 standardına uygun şekilde tamamlandı.
