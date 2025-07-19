## **Task 7**
1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```
CREATE TABLE employee (
	id SERIAL PRIMARY KEY,
	name VARCHAR(50) not null,
	birthday DATE,
	email VARCHAR(100)
);
```
2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```
insert into employee (name, birthday, email) values ('Lynett', '1919-02-22', 'lkoppelmann0@blog.com');
insert into employee (name, birthday, email) values ('Henri', '1966-01-07', 'hmaker1@huffingtonpost.com');
insert into employee (name, birthday, email) values ('Field', '1964-02-19', 'fdeakins2@examiner.com');
insert into employee (name, birthday, email) values ('Rosanne', '1955-02-19', 'rgodspede3@over-blog.com');
insert into employee (name, birthday, email) values ('Cathlene', '1949-02-16', 'cbaldacchi4@reference.com');
insert into employee (name, birthday, email) values ('Ron', '1985-10-08', 'rgarman5@storify.com');
insert into employee (name, birthday, email) values ('Jemmy', '1936-10-10', null);
insert into employee (name, birthday, email) values ('Carita', '1969-08-12', null);
insert into employee (name, birthday, email) values ('Samuele', '1935-07-26', 'sbrayshay8@sohu.com');
insert into employee (name, birthday, email) values ('Aubert', '1984-08-15', 'alehon9@elegantthemes.com');
insert into employee (name, birthday, email) values ('Lucine', '1916-12-06', 'lbewlya@sbwire.com');
insert into employee (name, birthday, email) values ('Maryjane', '1980-07-24', 'mgallacciob@digg.com');
insert into employee (name, birthday, email) values ('Brigitte', '1967-12-26', 'bkratesc@storify.com');
insert into employee (name, birthday, email) values ('Kinny', '1927-03-07', null);
insert into employee (name, birthday, email) values ('Tymon', '1952-11-02', 'tcisece@yahoo.com');
insert into employee (name, birthday, email) values ('Jeremie', '1938-01-17', null);
insert into employee (name, birthday, email) values ('Jennee', '1938-05-31', 'jsenterg@oracle.com');
insert into employee (name, birthday, email) values ('Skye', '1901-10-01', 'ssewallh@yolasite.com');
insert into employee (name, birthday, email) values ('Kaitlyn', '1982-04-18', 'kwhitbreadi@biblegateway.com');
insert into employee (name, birthday, email) values ('Steward', '1931-08-17', 'soxbiej@nih.gov');
insert into employee (name, birthday, email) values ('Karolina', '1972-10-07', 'kmattheissenk@google.fr');
insert into employee (name, birthday, email) values ('Blondell', '1968-04-03', 'bwoodhalll@blinklist.com');
insert into employee (name, birthday, email) values ('Jeromy', '1976-04-18', 'jjudem@e-recht24.de');
insert into employee (name, birthday, email) values ('Jania', '1953-05-10', 'jmacgraithn@cafepress.com');
insert into employee (name, birthday, email) values ('Rowen', '1955-04-12', 'rbloxholmo@ucoz.ru');
insert into employee (name, birthday, email) values ('Leonhard', '1933-02-22', 'lredmaynep@ustream.tv');
insert into employee (name, birthday, email) values ('Gerianna', '1998-07-02', 'ghebdenq@studiopress.com');
insert into employee (name, birthday, email) values ('Tonie', '1928-03-21', 'tpagetr@accuweather.com');
insert into employee (name, birthday, email) values ('Eleonore', '1993-07-27', 'eregis@amazonaws.com');
insert into employee (name, birthday, email) values ('Feliks', '1949-05-26', 'famiablet@godaddy.com');
insert into employee (name, birthday, email) values ('Eugenie', '1927-11-28', 'eusbornu@timesonline.co.uk');
insert into employee (name, birthday, email) values ('Gerianna', '1928-03-20', 'gshalloev@multiply.com');
insert into employee (name, birthday, email) values ('Bradly', '1918-03-29', 'bmcfaulw@thetimes.co.uk');
insert into employee (name, birthday, email) values ('Gil', '1960-03-09', 'gfossickx@mysql.com');
insert into employee (name, birthday, email) values ('Pattie', '1929-03-06', 'pfellonay@amazon.com');
insert into employee (name, birthday, email) values ('Enrika', '1977-03-08', 'epetrussiz@pagesperso-orange.fr');
insert into employee (name, birthday, email) values ('Tobe', null, 'tbroddle10@macromedia.com');
insert into employee (name, birthday, email) values ('Calida', '1976-12-04', 'cdando11@huffingtonpost.com');
insert into employee (name, birthday, email) values ('Sherri', '1986-09-12', 'saarons12@whitehouse.gov');
insert into employee (name, birthday, email) values ('Sinclare', '1994-07-13', 'spifford13@wiley.com');
insert into employee (name, birthday, email) values ('Selinda', '1958-06-17', 'sgogan14@yelp.com');
insert into employee (name, birthday, email) values ('Oneida', '1993-05-14', 'obygrave15@washingtonpost.com');
insert into employee (name, birthday, email) values ('Clarisse', '1973-08-29', 'cmulliner16@csmonitor.com');
insert into employee (name, birthday, email) values ('Cosetta', '1924-08-23', 'clanchbury17@examiner.com');
insert into employee (name, birthday, email) values ('Antoine', '1983-10-01', 'aswynfen18@weebly.com');
insert into employee (name, birthday, email) values ('Faunie', '1918-11-22', null);
insert into employee (name, birthday, email) values ('Kelcey', '1963-09-17', 'kproschke1a@webeden.co.uk');
insert into employee (name, birthday, email) values ('Anya', '1969-10-08', 'alile1b@pen.io');
insert into employee (name, birthday, email) values ('Michale', '1902-06-30', 'mgribbon1c@buzzfeed.com');
insert into employee (name, birthday, email) values ('Jo ann', '1943-05-04', 'jfeckey1d@sciencedirect.com');
```
3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```
UPDATE employee
SET name = 'Blair',
	birthday = '1997-08-28',
	email = 'blair@blog.com'
WHERE id = 2
RETURNING *;

UPDATE employee
SET name = 'XXXX'
WHERE name LIKE 'G%'
RETURNING *;

UPDATE employee
SET birthday = '2001-06-02'
WHERE id BETWEEN 6 AND 10
RETURNING *;

UPDATE employee
SET name = 'Old'
WHERE birthday < '1985-01-01'
RETURNING *;

UPDATE employee
SET name = 'Retired Eleonore'
WHERE email = 'eregis@amazonaws.com'
RETURNING *;
```
4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```
DELETE FROM employee
WHERE id = 2
RETURNING *;

DELETE FROM employee
WHERE id BETWEEN 3 AND 6
RETURNING *;

DELETE FROM employee
WHERE birthday < '1925-01-01'
RETURNING*;

DELETE FROM employee
WHERE email ILIKE 'S%' AND birthday BETWEEN '1950-01-01' AND '1990-01-01'
RETURNING*;

DELETE FROM employee
WHERE name = 'Old'
RETURNING*;
```