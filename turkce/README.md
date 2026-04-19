# Trello API Test Projesi (Turkce Ozet)

Bu klasor, ana projedeki Ingilizce dokumantasyonun Turkce ozetini icerir.

## Proje Amaci

Postman kullanilarak Trello API uzerinde su islemler test edildi:

- Pano olusturma
- Liste olusturma (sol/ust ve sag/alt)
- Kart olusturma
- Kart silme
- Pano bilgisi cekme
- Pano guncelleme

API key ve token ile guvenli erisim saglandi.
Response dogrulugu ve sure kontrolleri ile test kalitesi artirildi.

## Test Sonuc Ozeti

- 8 gorevin tamami basariyla tamamlandi.
- Her istekte beklenen HTTP durum kodlari alindi.
- Sure kontrolleri esik degerler altinda gecti (genel olarak < 500 ms, guncelleme istegi < 400 ms).
- Kanit dosyalari evidence/ klasorunde task-01-create-board.html - task-08-update-board.html olarak mevcuttur.

## Dosyalar

- Bu klasorde Turkce ozet bulunur.
- Ana teknik detaylar icin ust dizindeki README.md ve docs/ klasorune bakabilirsiniz.
