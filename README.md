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





















































