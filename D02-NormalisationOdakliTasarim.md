***WorkShop1: Udemy gibi bir sistemin veritabanını kurmak istiyoruz. Gereksinimler;
Kurs bilgilerini tutmak istiyoruz. Eğitmen bilgilerini tutmak istiyoruz. Bir kursun sadece bir Eğitmeni olacak.

![Ekran Alıntısı1](https://user-images.githubusercontent.com/77534195/188453310-178ee431-b696-4ed1-9bd6-e4834b9670a6.PNG)

Bu kısımda dikkat edeceğimiz şey eğitmen bir kere olabilir. Ancak eğitmenin birden fazla kursu olabilir.

***WorkShop2: Udemy gibi bir sistemin veritabanını kurmak istiyoruz. Önceki örnekten tek farkı; bir kursun bir veya birden fazla eğitmeni olabilir.

![Ekran Alıntısı2](https://user-images.githubusercontent.com/77534195/188454641-181af102-f6b8-4424-b37f-839163fe0077.PNG)

Kurslar tablosundaki Id ve Kurs Eğitmenleri tablosundaki KursId arasında one to many yani bireçok ilişki vardır.
Eğitmenler tablosundaki Id ve Kurs Eğitmenleri tablosundaki EğitmenId arasında one to many yani bireçok ilişki vardır.
