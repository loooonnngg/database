#week 4

###assignment 1
select country.name as "country name", airport.name as "airport name"
from country inner join airport on airport.iso_country = country.iso_country
where country.name = "Finland" and scheduled_service = "yes";
![img.png](image/img4-1.png)

###assignment 2
select screen_name, airport.name
from game inner join airport on location = ident;
![img.png](image/img4-2.png)

###assignment 3
select screen_name, country.name
from game inner join airport on location = ident inner join country on airport.iso_country = country.iso_country;
![img.png](image/img4-3.png)

###assignment 4
select airport.name, screen_name
from airport left join game on ident = location where name like "%Hels%";
![img.png](image/img4-4.png)

###assignment 5
select name, screen_name
from goal left join goal_reached on goal.id = goal_id  left join game on game.id = game_id;
![img.png](image/img4-5.png)