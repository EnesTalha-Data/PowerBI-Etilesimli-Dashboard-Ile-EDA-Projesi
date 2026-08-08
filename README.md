# PowerBI Etkileşimli Dashboard İle EDA Projesi
Bu projede PowerBI kullanarak etkileşimli bir dashboard oluşturdum ve bu dashboard aracılığı ile keşifçi veri analizi yaparak çeşitli bölgelerin ciroları, yoğunlukları ve başarı oranları gibi değişkenleri inceleyip yorumladım.

Burada amacım hangi bölgelerin en yüksek cirolara ulaştıklarını hangi bölgelerin yoğunluklarının en fazla olduğunu ve bölgelerin başarı oranlarını ve günlere göre değişimlerini inceleyerek yorumda bulunmak ve analiz etmektir.

Bu proje için PowerBI tercih etme sebebim; etkileşimli, şık ve kolay kullanımı olan bir proje hazırlamak istememdir.

NOT: Projede kullanılan veri tamamen anonimleştirilmiştir ve gerçeği yansıtmamaktadır.

# Dashboard Arayüzünü İnceleyelim

Öncelikle bu dashboard için hareketli bir arkaplan tercih ettim ve grafikleri, kartları ve dilimleyicileri oluştururken bu arkaplana uygun renkler kullandım. Böylece şık ve fazla renk karmaşası olmayan bir dashboard oluşmuş oldu.

Şimdi dilimleyiciler ile başlayalım;

<img width="1540" height="862" alt="Dilimleyici" src="https://github.com/user-attachments/assets/371da718-ad21-4887-a6ac-d98d5cb9de76" />

- Yukarıdaki resimde kırmızı ok ile gösterilen dilimleyici hangi bölgeye ait grafikleri ve kartları görebileceğimizi seçeceğimiz bir dilimleyicidir. Halihazırda Bölge_01'in seçili olduğunu görebiliyoruz. Ayrıca bu projede 38 farklı bölge yer almıştır.

<img width="1537" height="860" alt="Dilimleyici2" src="https://github.com/user-attachments/assets/da7bffd4-03fc-443a-aa10-9fd9f1780605" />

- Yine yukarıdaki görselde kırmızı ok ile gösterilen bir diğer dilimleyici ise 16 Haziran 2026 ve 3 Temmuz 2026 aralığındaki tarihleri kapsayan bir tarih dilimleyicisi. Bu kullanılarak hangi tarih aralığındaki verileri görmek istediğimizi ayarlayabiliyoruz.

Şimdi kartları inceleyelim;

<img width="1537" height="863" alt="Kart" src="https://github.com/user-attachments/assets/e704179b-d502-4ccc-81e9-c8ce7ea90ef3" />

- Yukarıda kırmızı ok ile gösterilen kart, seçilen bölgenin halka açık veya özel bölge olup olmadığını gösteren bir karttır. Eğer "Halka Açık" yazıyorsa bu bölge halkın kullanımına açık, "Özel" yazıyorsa sadece üye olanların kullanabildiği bir bölgedir. Bu kart önemlidir çünkü o bölgenin halka açık veya özel olması ciro ve yoğunluk gibi değişkenleri etkileyebilir.

<img width="1538" height="862" alt="Kartlar" src="https://github.com/user-attachments/assets/cae31248-00bf-4dd9-a046-cff2d747b327" />

- Bu görselde ise gösterilen kartlar seçilen bölgede bulunan cihaz türlerinin sayılarını gösterir. Mesela şuan Bölge_01 seçili iken "Cihaz 1" türünde 2 adet, "Cihaz 2" türünde 6 adet, "Cihaz 3" türünde 3 adet, "Cihaz 4" türünde 2 adet ve "Cihaz 5" türünde ise 1 adet cihaz olduğunu görüntüleyebiliyoruz. Bölgelerin cihaz sayılarının fazla veya az olması o bölgenin büyüklüğünü anlamamızı sağlayabilir.

Artık grafikleri inceleyebiliriz;

<img width="1538" height="862" alt="Grafik1" src="https://github.com/user-attachments/assets/e127470d-c71f-45af-989f-8621156aaf9f" />

- İlk grafiğimiz bir çizgi grafiğidir ve görselde kırmızı ok ile gösterilmiştir. Bu grafikte seçtiğimiz bölgenin hangi günlerde ne kadar ciro yaptığını ve yaptığı bu cironun ne kadarlık bir kısmının ödemesinin alınamadığını görebiliyoruz.
- Bu grafikte görülen turkuaz çizgi toplam ciroyu, lacivert çizgi ise ödeme alınamayan miktarı gösterir. (TL cinsinden)
- Eğer toplam ciro ve ödeme alınamayan çizgisi birbirine yakın değerlerde ise, o gün başarı oranımız o kadar düşüktür demektir. Yani mesela grafiği incelediğimizde Bölge_13 için 21 Haziran ve 28 Haziran tarihleri arasında birkaç günde iki çizgi iç içe geçmiştir. Bu demek oluyor ki o günlerde yaptığımız cironun hiçbir kısmının ödemesini alamamışız.
- Kısacası bu grafikten yola çıkarak hangi günlerde ne kadar ödemenin hatalı veya başarısız olduğunu görebilir ve bunu daha detaylı araştırabiliriz. Aynı zamanda hangi günlerde ne kadar ciro yaptığımızı görerek o günlerin analizini yapabiliriz.

<img width="1537" height="861" alt="Grafik2" src="https://github.com/user-attachments/assets/afc4b6ef-8993-4501-a75d-d756c3df97de" />

- Yukarıda kırmızı ok ile gösterilen bir diğer grafik ise bir alan grafiğidir. Bu grafikte seçtiğimiz bölgenin belirlediğimiz tarih aralığındaki başarı oranlarını görebiliyoruz.
- Örneğin görselde Bölge_13 için olan grafiği incelediğimizde 22 ve 25 Haziran tarihleri arasında başarı oranlarımızın 0 olduğunu görüyoruz. Yani bir önceki çizgi grafiğinde incelediğimiz durumu destekliyor. Bununla beraber 29 Haziran gününde başarı oranımızın 1 olduğunu yani mükemmel olduğunu görebiliyoruz.
- Bu grafiğin amacı hem bir önceki çizgi grafiğini desteklemek hem de başarı oranlarının hangi günler düşüş yaşadığını görebilmek, buna neyin sebep olduğunu inceleyebilmek ve araştırabilmektir.

<img width="1538" height="862" alt="Grafik3" src="https://github.com/user-attachments/assets/c1c8970d-a003-44a7-93f9-0277a13c146a" />

- Bir diğer grafiğimiz ise bir pasta grafiğidir. Bu grafik en yoğun 5 bölgeyi göstermek amacıyla yapılmıştır.
- Bölge dilimleyicisinin bu grafikte bir görevi yoktur çünkü bu grafik genel bir sıralama gösterir.
- Görselde görüldüğü üzere seçilen tarih aralığında toplam 78 bin giriş çıkış sayısı ile Bölge_22 en yoğun bölge olmuştur.
- Bu grafikten ise hangi bölgelerin ne kadar yoğun olduğunu inceleyebilir, diğer grafiklerden de yaralanarak yoğunluğun başarı oranına veya toplam ciroya etkisi var mı inceleyebiliriz.

<img width="1537" height="862" alt="Grafik4" src="https://github.com/user-attachments/assets/27f6daa7-e727-4f51-85e5-2a4bcc9396e8" />

- Bu grafik ise bir çubuk grafiğidir ve yine bölge dilimleyicisinden bağımsız çalışır. 
- Grafiğin amacı seçilen tarih aralığında bölgelerin başarı oranlarının ortalamasını almak ve bunları sıralamaktır.
- Görselde görüldüğü üzere seçtiğimiz tarih aralığında başarı ortalaması en yüksek olan bölge Bölge_24 olmuştur. (%99.4)
- Bu grafikten ise başarı oranı ortlaması olarak hangi bölgelerin en iyi olduklarını görebilir ve bu bölgelerin başarılarını ve bu başarıların sebeplerini inceleyebiliriz.




