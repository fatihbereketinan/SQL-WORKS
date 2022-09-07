***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql


1. Product tablosundaki ürün isimlerini getirdik. Products'a p takma adı verildi.

Select p.ProductName from Products p

2. Her bir ürünün tüm stoğunu satarsam total kazancım kaç olur?

Select p.ProductName, p.UnitsInStock * p.UnitPrice as Total from Products p

3. Metinsel ifadelere sahip kolonları yan yana getirelim.

Select p.ProductName + '-' + p.QuantityPerUnit from Products as p
