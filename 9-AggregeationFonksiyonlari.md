***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. COUNT: Bu fonksiyon ile belirtilen alandaki veya tablodaki toplam kayıt sayısını öğreniriz. 

Select Count(*) as [Ürün Sayısı] from Products
Select Count(ProductName) from Products
Select Count(*) from Customers
Select Count(Region) from Customers

2. SUM : Bu fonksiyon ile belli bir grup içinde toplama yapabiliriz.

Select Sum(UnitPrice) from [Order Details]

3. AVG : Bu fonksiyon belli bir grup içindeki sayısal değerlerin ortalamasını bize geri döndürür.

Select Avg(UnitPrice) from Products

4. MAX : Bu fonksiyon bir alan içindeki en büyük sayısal değeri geri döndürür.

Select Max(UnitPrice) from Products

5. MIN : Bu fonksiyon bir alan içindeki en küçük sayısal değeri geri döndürür.

Select Min(UnitPrice) from Products

6. RAND : Bu fonksiyon rastgele sayı üretir.

Select Rand()
