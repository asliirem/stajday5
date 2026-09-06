# HTTP Durum Kodları (Status Codes) - Notlar

API isteklerine karşılık dönen Response'ların başında bulunan durum kodları,
işlemin sonucu hakkında bilgi verir.

## Başarılı Durum Kodları (2xx)

| Kod | Anlamı        | Ne Zaman Alınır                                   |
|-----|---------------|----------------------------------------------------|
| 200 | OK            | GET isteği başarılı şekilde tamamlandığında         |
| 201 | Created       | POST isteğiyle yeni bir kayıt başarıyla oluştuğunda |
| 204 | No Content    | DELETE isteği başarılı, dönecek veri olmadığında    |

## İstemci Hataları (4xx)

| Kod | Anlamı        | Ne Zaman Alınır                                          |
|-----|---------------|-------------------------------------------------------------|
| 400 | Bad Request   | İstek gövdesinde eksik/hatalı bilgi gönderildiğinde          |
| 401 | Unauthorized  | Kimlik doğrulama bilgisi eksik veya geçersiz olduğunda        |
| 404 | Not Found     | İstenen kayıt (ör. ürün, müşteri) sistemde bulunamadığında     |

## Sunucu Hataları (5xx)

| Kod | Anlamı                | Ne Zaman Alınır                                  |
|-----|------------------------|----------------------------------------------------|
| 500 | Internal Server Error  | Sunucu tarafında beklenmeyen bir hata oluştuğunda   |

## Notlar

- Response içeriğini incelerken önce **durum kodu**na, sonra **body** içindeki
  verilere/mesaja bakmak hatayı hızlı tespit etmeyi sağlar.
- Postman'de gönderilen her istekten sonra sağ üstte durum kodu ve süre bilgisi görüntülenir.
- Başarılı isteklerde dönen veri genellikle JSON formatındadır; hata durumlarında
  ise açıklayıcı bir `mesaj` alanı bulunur.
