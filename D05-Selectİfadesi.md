***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Select bir veya bir den fazla tablodan veri çekmeye yarar. İlk örnekte product tablosunu getirdik.

Select * from Products

2. Product tablosuna ait bazı kolonları getirdik. 

Select ProductID, ProductName from Products

3. Product tablosuna ait getirdiğimiz kolonlara takma isim verdik. 

Select ProductID as Id, ProductName as Name from Products
