***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Inner Join: Ortak noktaya göre tabloları sadece eşleşenler üzerinden biraraya geririr.

*Ürünler tablosunda Categoryi görmek istiyorum?

Select*from Products p inner join Categories c on p.CategoryId=c.CategoryId

Select*from Products p inner join Categories c on p.CategoryId=c.CategoryId where p.UnitPrice>20 order by c.CategoryId

*Birden çok tabloyla join yapmak istiyorum

Select p.ProductName, o.OrderDate, od.Quantity*od.UnitPrice as Total from Products p inner join [Order Details] od on p.ProductId=od.ProductId inner join Orders o on o.OrderId=od.OrderId order by p.ProductName, o.OrderDate

2. Left Join: Soldaki tabloda olup sağdaki tabloda olmayanlarıda getirir. Yani solda eşleşmeyenlerde gelir.

Stoğumuz da satamadığımız ürünler hangileridir?

Select * from Products p left join [Order Details] od on p.ProductId=od.ProductId where od.ProductId is null

Hiç satış yapmadığımız müşterilerimiz hangileridir?

Select * from Customers c left join Orders o on c.CustomerId=o.CustomerId where o.CustomerId is null

3. Right Join: Sağdaki tabloda olup soldaki tabloda olmayanlarıda getirir. Yani sağda eşleşmeyenlerde gelir. Left Joinin tam tersidir.

Select c.ContactName, c.CustomerId from Orders o right join Customers c on o.CustomerId=c.CustomerId where o.CustomerId is null

4. Full Join: inner, left, right hepsi gelir. Yani eşleşen artı eşleşmeyelenlerin tamamı tabloda yer alır.

Select * from Customers c full join Orders o on o.CustomerId=c.CustomerId



