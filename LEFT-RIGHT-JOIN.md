1:city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
----------------------------------------------------------------------
SELECT city, country FROM country
LEFT JOIN city ON city.country_id = country.country_id;
----------------------------------------------------------------------
2:customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
----------------------------------------------------------------------
SELECT first_name, last_name, payment_id FROM payment
LEFT JOIN customer ON customer.customer_id = payment.customer_id;
----------------------------------------------------------------------
3:customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
----------------------------------------------------------------------
SELECT first_name, last_name, rental_id FROM rental
FULL JOIN customer ON customer.customer_id = rental.rental_id;
----------------------------------------------------------------------
