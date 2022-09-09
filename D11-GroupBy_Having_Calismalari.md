***Çalışmalar Microsoft'un örnek veri tabanı olan Northwind üzerinden yapılmıştır. 
https://raw.githubusercontent.com/microsoft/sql-server-samples/master/samples/databases/northwind-pubs/instnwnd.sql

1. Discint: Bir kolondaki tekrarlayan kayıtları tekrarsız halde getirir.

Select discint(Country) from Customers order by Country

Select discint Country, City from Customers order by Country ---iki kolonu birlikte tekrarsız halde getirir.

2. Group By: Belirtilen kolon veya kolonlara göre aynı değere sahip verileri gruplar.

Select Country from Customers group by Country

Select Country, Count(*) from Customers group by Country

Select Country, City, Count(*) from Customers group by Country,City

3. Having: where komutu gruplama fonksiyonları ile kullanılmadığından aynı görevi yapan having komutu group by ile kullanılması için getirilmiştir.

--Ülke şehir bazında birden fazla müşterilemiz nerelerde var ?

Select Country, City, Count(*) from Customers group by Country,City having Count(*)>1 order by Country

Select Country, City, Count(*) from Customers where City<>'Nantes' group by Country,City having Count(*)>1 order by Country

