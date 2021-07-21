# Patika-SQL
### Patika.dev tarafindan hazirlanan SQL egitim serisinin ödevleri

## 1.Ödev

```bash
select title, description from film
```
```bash
select * from film where length between 60 and 75
```

```bash
select * from film where rental_rate = 0.99 AND replacement_cost = 12.99 OR replacement_cost = 28.99

```

```bash
select last_name from customer where first_name = 'Mary'
Smith
```
```bash
select * from film where  length < 50 AND  NOT rental_RATE = 2.99 OR NOT rental_rate = 4.99
```

## 2.Ödev
```bash
select * from film where replacement_cost between 12.99 and 16.99 

```
```bash
select first_name,last_name from Actor where first_name in('Penelope','Nick','Ed')
```
```bash
select * from film where rental_rate in(0.99,2,99,4,99) and replacement_cost in(12.99,15.99,28.99)

```

## 3.Ödev
```bash
select * from country where country like 'A%a'

```
```bash
select * from country where country like '______%n'
```
```bash
select title from film where title like '%t%t%t%t%'

```
```bash
select * from film where title like 'C%' and length > 90 and rental_rate = 2.99 

```

## 4.Ödev
```bash
select distinct replacement_cost from film  

```
```bash
select count(distinct replacement_cost ) from film 
```
```bash
select count(*) from film where title like 'T%' and rating = 'G'

```
```bash
select count(*) from country where country like '_____'

```
```bash
select count(*) from city where city like 'R%r'
```

## 5.Ödev
```bash
select title from film where title like '%n' order by length desc limit 5

```
```bash
select title from film where title like '%n' order by length  limit 5

```
```bash
select title from film where title like '%n' order by length  limit 5  offset 6

```
```bash
select * from customer  where store_id = 1 order by last_name desc limit 4 
```
## 6.Ödev
```bash
select avg(rental_rate) from film

```
```bash
select count(*) from film where title like 'C%'


```
```bash
select length from film  where rental_rate = 0.99  order by length desc limit 1


```
```bash
select count(distinct replacement_cost) from film  where length>150
```


## 7.Ödev
```bash
select rating from film group by rating

```
```bash
select replacement_cost, count(*)   from film group by replacement_cost having count(*) > 50


```
```bash
select store_id, count(*) from customer group by store_id  


```
```bash
select country_id , count(*) from city group by country_id  ORDER BY COUNT(country_id) DESC limit 1

```


## 8.Ödev
```bash
create table employee(

	id integer,
	name varchar(50),
	birthday date,
	email varchar(100)
)
```
```bash
insert into employee (id, name, email, birthday) values (1, 'Gunter', 'gtackle0@tinyurl.com', '21/1/1994');
insert into employee (id, name, email, birthday) values (2, 'Caryn', 'churran1@webs.com', '5/7/2007');
insert into employee (id, name, email, birthday) values (3, 'Robbie', 'rdockerty2@oakley.com', '3/2/2019');
insert into employee (id, name, email, birthday) values (4, 'Alethea', 'adan3@mapy.cz', '25/3/2004');
insert into employee (id, name, email, birthday) values (5, 'Zora', 'zcleef4@istockphoto.com', '5/10/2002');
insert into employee (id, name, email, birthday) values (6, 'Violette', 'vneles5@scientificamerican.com', '19/3/1996');
insert into employee (id, name, email, birthday) values (7, 'Timothy', 'tspelsbury6@google.com.hk', '14/10/1992');
insert into employee (id, name, email, birthday) values (8, 'Guthrie', 'giliff7@gov.uk', '10/4/2011');
insert into employee (id, name, email, birthday) values (9, 'Milena', 'msheeres8@moonfruit.com', '29/7/1983');
insert into employee (id, name, email, birthday) values (10, 'Eilis', 'ejaslem9@wikispaces.com', '4/10/1982');
insert into employee (id, name, email, birthday) values (11, 'Wallas', 'wrippera@europa.eu', '12/10/1987');
insert into employee (id, name, email, birthday) values (12, 'Phylis', 'pdoohanb@g.co', '24/11/2008');
insert into employee (id, name, email, birthday) values (13, 'Basilius', 'bcroneyc@cloudflare.com', '10/6/1992');
insert into employee (id, name, email, birthday) values (14, 'Reba', 'rrettied@cyberchimps.com', '23/3/1987');
insert into employee (id, name, email, birthday) values (15, 'Sherye', 'sroebottome@dell.com', '2/9/1997');
insert into employee (id, name, email, birthday) values (16, 'Pearce', 'pjentgensf@purevolume.com', '27/1/2019');
insert into employee (id, name, email, birthday) values (17, 'Mathilda', 'mfeltong@virginia.edu', '6/5/1988');
insert into employee (id, name, email, birthday) values (18, 'Laughton', 'lwattingh@huffingtonpost.com', '5/6/1997');
insert into employee (id, name, email, birthday) values (19, 'Julie', 'jscriveni@upenn.edu', '28/2/1985');
insert into employee (id, name, email, birthday) values (20, 'Archaimbaud', 'apabstj@amazon.co.jp', '28/6/1993');
insert into employee (id, name, email, birthday) values (21, 'Janella', 'jmateik@baidu.com', '30/12/1988');
insert into employee (id, name, email, birthday) values (22, 'Vernon', 'vmcquakerl@moonfruit.com', '23/12/2004');
insert into employee (id, name, email, birthday) values (23, 'Ransell', 'rhorwellm@zimbio.com', '1/12/1997');
insert into employee (id, name, email, birthday) values (24, 'Rafaelita', 'rdetloffn@oaic.gov.au', '29/12/2012');
insert into employee (id, name, email, birthday) values (25, 'Buddy', 'bkirwoodo@amazon.com', '11/8/2009');
insert into employee (id, name, email, birthday) values (26, 'Bran', 'bverrechiap@last.fm', '9/12/1982');
insert into employee (id, name, email, birthday) values (27, 'Bjorn', 'bhoonahanq@wiley.com', '12/2/2013');
insert into employee (id, name, email, birthday) values (28, 'Ferdinanda', 'fsperryr@bloglines.com', '22/2/2006');
insert into employee (id, name, email, birthday) values (29, 'Seth', 'scapess@fastcompany.com', '3/4/1987');
insert into employee (id, name, email, birthday) values (30, 'Donnamarie', 'dgonthardt@is.gd', '31/10/2013');
insert into employee (id, name, email, birthday) values (31, 'Myriam', 'mgutchu@people.com.cn', '24/3/1995');
insert into employee (id, name, email, birthday) values (32, 'Maressa', 'mandrivotv@unicef.org', '9/11/1995');
insert into employee (id, name, email, birthday) values (33, 'Clemmie', 'cvermerw@yandex.ru', '23/9/1990');
insert into employee (id, name, email, birthday) values (34, 'Shalom', 'skelshawx@sciencedaily.com', '31/12/1985');
insert into employee (id, name, email, birthday) values (35, 'Charlie', 'cbrowelly@google.it', '1/12/2013');
insert into employee (id, name, email, birthday) values (36, 'Glynis', 'gharriez@google.pl', '20/8/1991');
insert into employee (id, name, email, birthday) values (37, 'Robenia', 'rwilber10@google.co.uk', '1/11/2001');
insert into employee (id, name, email, birthday) values (38, 'Elbertina', 'edibbert11@webs.com', '25/9/1981');
insert into employee (id, name, email, birthday) values (39, 'Nita', 'narno12@pbs.org', '7/6/1990');
insert into employee (id, name, email, birthday) values (40, 'Ailyn', 'aleggs13@liveinternet.ru', '21/1/1999');
insert into employee (id, name, email, birthday) values (41, 'Connie', 'cdurno14@comcast.net', '5/9/1991');
insert into employee (id, name, email, birthday) values (42, 'Staford', 'sohingerty15@nbcnews.com', '5/6/2011');
insert into employee (id, name, email, birthday) values (43, 'Annamarie', 'abanck16@fda.gov', '14/2/2021');
insert into employee (id, name, email, birthday) values (44, 'Roxane', 'rrosenblad17@reverbnation.com', '27/8/2005');
insert into employee (id, name, email, birthday) values (45, 'Culley', 'cmollatt18@networkadvertising.org', '28/2/2003');
insert into employee (id, name, email, birthday) values (46, 'Westbrooke', 'wgierhard19@toplist.cz', '14/11/2003');
insert into employee (id, name, email, birthday) values (47, 'Kati', 'kmertin1a@apache.org', '21/2/2000');
insert into employee (id, name, email, birthday) values (48, 'Bevon', 'bbraxton1b@mapy.cz', '24/7/1994');
insert into employee (id, name, email, birthday) values (49, 'Reagen', 'rmallett1c@tumblr.com', '28/9/2010');
insert into employee (id, name, email, birthday) values (50, 'Peg', 'panthonies1d@nifty.com', '31/3/1991');



```
```bash
UPDATE Employee SET name = 'Fatih' WHERE id = 1
UPDATE Employee SET email = 'fatih-348@hotmail.com' WHERE name = 'fatih'
UPDATE Employee SET birthday = '10/01/1996' WHERE email = 'fatih-348@hotmail.com'
UPDATE Employee SET email = 'fatihmutlu348@gmail.com', birthday = '01/01/1996' WHERE id = 1
UPDATE Employee SET name = 'Fatih Mutlu', email = 'fatihmutlu348@gmail.com'


```
```bash
DELETE FROM Employee WHERE name = 'Robbie';
DELETE FROM Employee WHERE email = '"rdockerty2@oakley.com"';
DELETE FROM Employee WHERE birthday = '"1992-10-14"';
DELETE FROM Employee WHERE name  like 'C____'
DELETE FROM Employee WHERE id = 11

```
## 9.Ödev
```bash
select city.city, country.country from city join  country on city.city = country.country

```
```bash
select city.city, country.country from city join  country on city.city = country.country


```
```bash
select customer.first_name, customer.last_name from customer join  rental on customer.rental_id  = rental.rental_id 

