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



