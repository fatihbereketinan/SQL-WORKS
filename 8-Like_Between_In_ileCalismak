***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Like operatörü tablomuzda bulunan kayıtlardan belirttiğimiz kriterler uygun olanları seçmek için kullanılır.

Select * from Products where ProductName like '%ch'
Select * from Products where ProductName like 'ch%'
Select * from Products where ProductName like '%ch%'

2. Between operatörü ile bir alanda belirtilen aralıktaki değerleri aramak için kullanılır.

Select * from Products where UnitPrice between 10 and 46 order by UnitPrice----Birim fiyatı 10 ile 46 arasında olanları getir.

3. In operatörü belirtilen tek bir alanda birden fazla değeri aramak için kullanılır.

Select * from Products where CategoryId in (1,2)------CategoryId'si 1 ve 2 olanları getir.
