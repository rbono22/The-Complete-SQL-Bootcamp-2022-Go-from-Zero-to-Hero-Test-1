# The-Complete-SQL-Bootcamp-2022-Go-from-Zero-to-Hero-Test-1

ASSESSMENT TEST 1

COMPLETE THE FOLLOWING TASKS!

* Return the customer IDs of customers who have spent at least $110 with the staff member who has an ID of 2.

SELECT customer_id,SUM(amount)<br>
FROM payment<br>
WHERE staff_id = 2<br>
GROUP BY customer_id<br>
HAVING SUM(amount) > 110;<br>
<br>
The answer should be customers 187 and 148

* How many films begin with the letter J? 

SELECT COUNT(*) FROM film<br>
WHERE title LIKE 'J%';<br>
<br>
The answer is 20


* What customer has the highest customer ID number whose name starts with an 'E' and has an address ID lower than 500?

SELECT first_name,last_name FROM customer<br>
WHERE first_name LIKE 'E%'<br>
AND address_id <500<br>
ORDER BY customer_id DESC<br>
LIMIT 1;<br>
<br>
The answer is Eddie Tomlin

