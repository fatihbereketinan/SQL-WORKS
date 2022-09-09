***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Left: İki parametre alır. İlk parametre bir string değer alır, ikinci parametre olarak bir int değer alır. Sonuç olarak int değeri kadar harfi stringin solundan döndürür.

Select Left(ProductName,3)

2. Right: Left fonksiyonu ile aynı çalışır. Farkı metni sağdan alıyor olmasıdır.

Select Right(ProductName,3)

3. Len: Parametre olarak aldığı string değerin uzunluğunu döndürür.

Select ProductName, Len(ProductName) as Karekter from Products

4. Lower: Parametre olarak aldığı stringin tümünü küçük harfe çevirerek dödürür.

Select Lower(ProductName) from Products

5. Upper: Lower ile aynı çalışır. Verilen stringin tamamını büyük harfe çevirir.

Select Upper(ProductName) from Products

6. Trim: Stringin hem sağ hem solundan boşlukları siler.

Select TRIM('     Fatih İnan    ')

7. LTRIM: Parametre olarak aldığı stringin solunda olan bütün boşlukları kaldırır.

Select LTRIM('     Fatih İnan    ')

8. RTRIM: Stringin sağındaki boşlukları siler.

Select RTRIM('     Fatih İnan    ')

9. REVERSE: Verilen string değeri ters çevirir.

Select REVERSE('     Fatih İnan    ')

10. CHARINDEX: Verilen iki parametreden ilk verilen değeri ikinci parametre içerisinde arar ve bulduğu ilk indeksi verir. Üçüncü parametre de isteğe bağlı ve verilmesi durumunda verilen indekten sonrası için arar. Aranan değer bulunmaz ise 0 değerini döner.

Select ProductName from Products where CHARINDEX(' ',ProductName,1)>0

11. REPLACE: Üç parametre alır. İkinci parametrede verilen string değeri birinci parametrede verilen string içerisinde arar ve üçüncü parametrede verilen değer ile değiştirir. Örneğin aşağıdaki örnekte “sai1orhan1” string değerinde geçen “1”leri “2” olarak değiştiriyor.

Select REPLACE(ProductName,' ','_') from Products

12. SUBSTRING: String içerisinden belli bir bölümü döndürür. Üç parametre alır. İlk parametrede işlem yapılacak string değeri, ikinci parametrede alınacak alt parçanın başladığı index değeri ve son parametre olarak da alınacak alt parçanın uzunluğunu alır.

Select SUBSTRING('Fatih İnan',2,5)

13. Ascii: Karekterin sayısal karşılığını verir.

Select Ascii('A')

14. Char: Değerin karekter karşılığını verir.

Select Char(65)
