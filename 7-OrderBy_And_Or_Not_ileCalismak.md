***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Şartları sağlayanları getir

Select * from Products where CategoryID=1 and SupplierID=1 

2. Stok adedi 10'dan büyük olan ürünleri getir.

Select * from Products where UnitsInStock>=10

3. Stokta olmayan ve sipariş bekleyen ürünleri getir.

Select * from Products where UnitsInStock=0 and UnitsOnOrder>0

4. Stokta olmayan veya sipariş bekleyen ürünleri getir.

Select * from Products where UnitsInStock=0 or UnitsOnOrder=0

5. Ürün adı Chai olmayan ve stoğu olmayan ürünleri getir.

Select * from Products where not ProductName='Chai' and UnitsInStock=0

6. Ürünler tablosunu ürün adına göre sırala. (asc:artanlı-----------desc:düşenli)

Select * from Products order by ProductName asc



--Şartlı şekilde filtreme yapacaksak where komutunu kullanırız.
