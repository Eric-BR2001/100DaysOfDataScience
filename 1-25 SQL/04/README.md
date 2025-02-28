# Cards Issued Difference
## JP Morgan SQL Interview Question

Your team at JPMorgan Chase is preparing to launch a new credit card, and to gain some insights, you're analyzing how many credit cards were issued each month.

### Problem Statement
Write a query that outputs the name of each credit card and the difference in the number of issued cards between the month with the highest issuance and the lowest issuance. Arrange the results based on the largest disparity.

### Table: `monthly_cards_issued`
| Column Name    | Type    |
|----------------|---------|
| card_name      | string  |
| issued_amount  | integer |
| issue_month    | integer |
| issue_year     | integer |

### Example Input

card_name               | issued_amount | issue_month | issue_year
------------------------|---------------|-------------|-----------
Chase Freedom Flex      | 55000         | 1           | 2021
Chase Freedom Flex      | 60000         | 2           | 2021
Chase Freedom Flex      | 65000         | 3           | 2021
Chase Freedom Flex      | 70000         | 4           | 2021
Chase Sapphire Reserve  | 170000        | 1           | 2021
Chase Sapphire Reserve  | 175000        | 2           | 2021
Chase Sapphire Reserve  | 180000        | 3           | 2021

### Example Output

card_name               | difference
------------------------|-----------
Chase Freedom Flex      | 15000
Chase Sapphire Reserve  | 10000

## My Solution:

SELECT card_name,MAX(issued_amount) - MIN(issued_amount) AS difference FROM monthly_cards_issued GROUP BY card_name ORDER BY 2 DESC;

### I used the fuction MAX, to get the max number. And I used the fuction MIN, to get the min number.  

# Cards Issued Difference
## JP Morgan SQL Interview Question

Your team at JPMorgan Chase is preparing to launch a new credit card, and to gain some insights, you're analyzing how many credit cards were issued each month.

### Problem Statement
Write a query that outputs the name of each credit card and the difference in the number of issued cards between the month with the highest issuance and the lowest issuance. Arrange the results based on the largest disparity.

### Table: `monthly_cards_issued`
| Column Name    | Type    |
|----------------|---------|
| card_name      | string  |
| issued_amount  | integer |
| issue_month    | integer |
| issue_year     | integer |

### Example Input

card_name               | issued_amount | issue_month | issue_year
------------------------|---------------|-------------|-----------
Chase Freedom Flex      | 55000         | 1           | 2021
Chase Freedom Flex      | 60000         | 2           | 2021
Chase Freedom Flex      | 65000         | 3           | 2021
Chase Freedom Flex      | 70000         | 4           | 2021
Chase Sapphire Reserve  | 170000        | 1           | 2021
Chase Sapphire Reserve  | 175000        | 2           | 2021
Chase Sapphire Reserve  | 180000        | 3           | 2021

### Example Output

card_name               | difference
------------------------|-----------
Chase Freedom Flex      | 15000
Chase Sapphire Reserve  | 10000

## My Solution:
SELECT drug, (total_sales - cogs) AS total_profit FROM pharmacy_sales ORDER BY total_profit DESC LIMIT 3;

### I use a simple sub and ask for order by total_profit with limit of 3 rows

---

## Battles in Game of Thrones

| Name | Year | Battle Number | Attacker King | Defender King | Attacker 1 | Attacker 2 | Attacker 3 | Attacker 4 | Defender 1 | Defender 2 | Defender 3 | Defender 4 | Attacker Outcome | Battle Type | Major Death | Major Capture | Attacker Size | Defender Size | Attacker Commander | Defender Commander | Summer | Location | Region | Note |
|------|------|---------------|---------------|---------------|------------|------------|------------|------------|------------|------------|------------|------------|-----------------|-------------|-------------|--------------|--------------|--------------|----------------|----------------|---------|----------|--------|------|
| Battle of the Golden Tooth | 298 | 1 | Joffrey/Tommen Baratheon | Robb Stark | Lannister |  |  |  | Tully |  |  |  | win | pitched battle | true | false | 15000 | 4000 | Jaime Lannister | Clement Piper, Vance | true | Golden Tooth | The Westerlands |  |
| Battle at the Mummer's Ford | 298 | 2 | Joffrey/Tommen Baratheon | Robb Stark | Lannister |  |  |  | Baratheon |  |  |  | win | ambush | true | false |  | 120 | Gregor Clegane | Beric Dondarrion | true | Mummer's Ford | The Riverlands |  |
| Battle of Riverrun | 298 | 3 | Joffrey/Tommen Baratheon | Robb Stark | Lannister |  |  |  | Tully |  |  |  | win | pitched battle | false | true | 15000 | 10000 | Jaime Lannister, Andros Brax | Edmure Tully, Tytos Blackwood | true | Riverrun | The Riverlands |  |
| Battle of the Green Fork | 298 | 4 | Robb Stark | Joffrey/Tommen Baratheon | Stark |  |  |  | Lannister |  |  |  | loss | pitched battle | true | true | 18000 | 20000 | Roose Bolton, Wylis Manderly, Medger Cerwyn, Harrion Karstark, Halys Hornwood | Tywin Lannister, Gregor Clegane, Kevan Lannister, Addam Marbrand | true | Green Fork | The Riverlands |  |
| Battle of the Whispering Wood | 298 | 5 | Robb Stark | Joffrey/Tommen Baratheon | Stark | Tully |  |  | Lannister |  |  |  | win | ambush | true | true | 1875 | 6000 | Robb Stark, Brynden Tully | Jaime Lannister | true | Whispering Wood | The Riverlands |  |



## Characters in Game of Thrones

| Birth Year | Character Name | Gender | House ID | Person ID |
|------------|---------------|--------|----------|-----------|
| 263 | Eddard Stark | M | 100 | 1 |
| 283 | Robb Stark | M | 100 | 2 |
| 286 | Sansa Stark | F | 100 | 3 |
| 291 | Tommen Baratheon | M | 400 | 32 |
|  | Stannis Baratheon | M | 400 | 33 |
|  | Renly Baratheon | M | 400 | 34 |
|  | Gendry | M | 400 | 35 |
|  | Barra | F | 400 | 36 |
|  | Edric Storm | M | 400 | 37 |
| 259 | Rhaegar Targaryen | M | 500 | 41 |
| 284 | Daenerys Targaryen | F | 500 | 44 |
|  | Viserys Targaryen | M | 500 | 45 |
| 198 | Maester Aemon | M | 500 | 46 |


## Animals in Game of Thrones

| Coloring | Gender | Name | Owner Person ID | Species | Weight | Weight Unit |
|----------|--------|------|----------------|---------|--------|-------------|
| grey | M | Grey Wind | 2 | direwolf | 400 | kg |
| brown, grey | F | Lady | 3 | direwolf | 350 | kg |
| brown, grey | F | Nymeria | 4 | direwolf | 300 | kg |
| black | M | Shaggydog | 6 | direwolf | 375 | kg |
| brown, grey | M | Summer | 5 | direwolf | 350 | kg |
| white | M | Ghost | 108 | direwolf | 400 | kg |
| black, red | M | Drogon | 44 | dragon | 28000 | kg |
| cream, gold, red, orange | M | Viserion | 44 | dragon | 25000 | kg |
| green, bronze, yellow, orange | M | Rhaegal | 44 | dragon | 23000 | kg |
| green, black | null | Unnamed Manticore |  | manticore | 2 | kg |
| black | null | Unnamed Shadowcat |  | shadowcat | 82 | kg |


select character_name from got_characters where character_name like "%Stark" order by 1
select character_name from got_characters where character_name LIKE "Jon%"
select character_name from got_characters where character_name LIKE "%ae%"
select * from gotcreatures where name like "%grey%"
select * from got_battles where attacker_1 like "%Baratheon%" and defender_king like "%Stark%"
select * from got_battles where summer=TRUE and attacker_king like "%Joffery%"