# Staj Günü 5 - Postman ile API Testi

Bu klasör, staj kapsamında Postman kullanılarak yapılan API test çalışmalarını içerir.

## İçerik

- **01_postman_collection.json** — Postman'e import edilebilir koleksiyon dosyası.
  GET (ürün listeleme, tek ürün görüntüleme) ve POST (müşteri ekleme, sipariş oluşturma)
  isteklerini içerir.
- **02_response_ornekleri.json** — Başarılı ve hatalı isteklere karşılık dönen örnek
  Response yapıları (200, 201, 400, 404, 500 durum kodlarıyla).
- **03_http_durum_kodlari.md** — HTTP durum kodlarının (status code) anlamları ve
  hangi durumlarda alındığına dair referans notu.

## Konu Özeti

- **Postman**: API servislerini test etmek için kullanılan, istek oluşturma ve
  Response inceleme imkânı sunan bir program.
- Bir isteğin doğru çalışması için: doğru adres, eksiksiz bilgi ve uygun HTTP
  metodunun seçilmesi gerekir.
- **Response** yapıları: Başarılı işlemlerde JSON formatında veri, hata durumlarında
  ise durum kodu ve açıklayıcı mesaj döner.
- **GET**: Veri listeleme/görüntüleme, **POST**: Yeni kayıt oluşturma amacıyla kullanılır.

## Nasıl Kullanılır

1. Postman programını açın.
2. `Import` butonuna tıklayıp `01_postman_collection.json` dosyasını seçin.
3. Koleksiyondaki istekleri tek tek göndererek Response'ları inceleyin.
4. `02_response_ornekleri.json` ve `03_http_durum_kodlari.md` dosyalarını referans
   olarak kullanarak gelen cevapları yorumlayın.
