#week 3

###assignment 1
select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = "Iceland";
![img.png](image/img3-1.png)

###assignment 2
select airport.name as 'airport name' from airport,country
where airport.iso_country=country.iso_country and country.name ='France' and airport.type='large_airport'
![img.png](image/img3-2.png)

###assignment 3
select country.name as country_name, airport.name as airport_name
from airport, country
where airport.iso_country = country.iso_country and country.continent = "AN";
![img.png](image/img3-3.png)

###assignment 4
select elevation_ft
from airport, game
where location = ident and screen_name = "Heini";
![img.png](image/img3-4.png)

###assignment 5
select 0.3048*elevation_ft as elevation_m 
from airport, game
where location = ident and screen_name = "Heini";
![img.png](image/img3-5.png)

###assignment 6
select airport.name
from airport, game
where location = ident and screen_name = "Ilkka";
![img.png](image/img3-6.png)

###assignment 7
select country.name
from airport, game, country
where location = ident and airport.iso_country = country.iso_country and screen_name = "Ilkka";
![img.png](image/img3-7.png)

###assignment 8
select name
from goal, goal_reached, game
where game.id = game_id and goal.id = goal_id and screen_name = "Heini";
![img.png](image/img3-8.png)

###assignment 9
select airport.name
from goal, goal_reached, game,airport
where game.id = game_id and goal.id = goal_id AND location = airport.ident and screen_name = "Ilkka";
![img.png](image/img3-9.png)

###assignment 10
SELECT country.name                                                                                                                                
from goal, goal_reached, game,airport,country                                                                                                      
where game.id = game_id and goal.id = goal_id AND location = airport.ident AND airport.iso_country = country.iso_country and screen_name = "Ilkka";
![img.png](image/img3-10.png)