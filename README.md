Question 1:
select * FROM actor;
Question 2:
select first_name FROM actor WHERE first_name = "John";
Question 3:
select last_name FROM actor WHERE last_name = "Neeson";
Question 4:
select actor_id FROM actor WHERE actor_id % 10 = 0 ORDER BY actor_id ASC;
Question 5:
select title, film_id FROM film WHERE film_id = 100;
Question 6:
select DISTINCT title, rating FROM film WHERE rating = "R";
Question 7:
select DISTINCT title, rating FROM film WHERE rating != "R";
Question 8:
select title, length FROM film ORDER BY length ASC LIMIT 10;
Question 9:
select title FROM film ORDER BY length ASC LIMIT 10;
Question 10:
select DISTINCT title, special_features FROM film WHERE special_features = "Deleted Scenes";
Question 11:
select DISTINCT last_name FROM actor;
Question 12: (come back if time)
select last_name, COUNT(last_name) AS Total FROM actor GROUP BY last_name ORDER BY Total DESC;
Question 13:
select fa.actor_id, COUNT(f.film_id) FROM film f JOIN film_actor fa ON fa.film_id = f.film_id GROUP BY fa.actor_id;
Question 14:
select i.store_id, f.title FROM inventory i JOIN film f ON i.film_id = f.film_id WHERE i.store_id = 1 AND f.title = "Academy Dinosaur";
Question 15:
select title, release_year FROM film WHERE title = "Academy Dinosaur";
Question 16:
select AVG(length) FROM film;
Question 17:
select fc.category_id, AVG(f.length) FROM film_category fc JOIN film f ON f.film_id = fc.film_id GROUP BY fc.category_id ASC;
Question 18:
select title FROM film WHERE title LIKE "%ROBOT%";
Question 19:
select title, length FROM film ORDER BY length DESC LIMIT 10;
Question 20: (come back later)
select release_year, COUNT(release_year) AS Total FROM film GROUP BY release_year;
Question 21:
select title, category FROM film_list WHERE category = "Horror";
Question 22:
select staff_id, first_name, last_name, CONCAT(first_name,' ', last_name) FROM staff WHERE staff_id = 1;
Question 23: 
select actor_id,first_name, last_name FROM actor WHERE first_name = "Fred"; (to get his ID)
select f.title, fa.actor_id FROM film_actor fa JOIN film f ON fa.film_id = f.film_id WHERE fa.actor_id = 16;
Question 24:
select film_id FROM film WHERE title = "BUCKET BROTHERHOOD"; (to get the film id)
Cannot find stock quantity....
Question 25:
select DISTINCT country_id,country FROM country;
select DISTINCT name, language_id FROM language ORDER BY name ASC;
Question 26:
select first_name, last_name FROM customer WHERE last_name LIKE "%son%" ORDER BY first_name;
Question 27:(didnt have time to create table but would have used this)
select category_id, COUNT(film_id) FROM film_category GROUP BY category_id;
Question 28: (this will help find 29) didnt have time to create new tables but would have used this 
select fa.actor_id, COUNT(f.film_id) AS Total FROM film f JOIN film_actor fa ON fa.film_id = f.film_id GROUP BY fa.actor_id ORDER BY Total ASC;
Question 29: 
select actor_id, first_name, last_name FROM actor WHERE actor_id = 107;
(GINA)

IF I had more time for question 7 i would have created the table or a new list to implement the category keys and number of films. then linked it to category to ensure that the names of the category is shown.

For question 8 I would create a table or a new list, and used the code shown above.

