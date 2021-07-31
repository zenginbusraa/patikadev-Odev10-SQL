1. soru : city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.

`` SELECT city.city ,country.country
FROM city
LEFT JOIN country ON country.country_id = city.country_id; ``


2. soru : customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

`` SELECT p.payment_id,c.first_name, c.last_name
FROM payment as p
RIGHT JOIN customer AS c ON c.customer_id = p.customer_id;  ``


3. soru : customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.


`` SELECT r.rental_id,c.first_name, c.last_name
FROM customer as c
FULL JOIN rental AS r ON c.customer_id = r.customer_id; ``