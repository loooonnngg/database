#Week 3

###assignment 1
select * from goal;
![img.png](image/img2-1.png)

###assignment 2
select name from airport where iso_country = "FI";
![img_1.png](image/img2-2.png)

###assignment 3
select name from airport where iso_country = "FI" order by name;
![img_2.png](image/img2-3.png)

###assignment 4
select name, type from airport where iso_country = "FI" order by type, name;
![img_3.png](image/img2-4.png)

###assignment 5
select name from country where name like "F%";
![img_4.png](image/img2-5.png)

###assignment 6
select name from country where name like "%F%";
![img_5.png](image/img2-6.png)

###assignment 7
select location from game where screen_name="Vesa";
![img_6.png](image/img2-7.png)

###assignment 8
select co2_consumed from game where screen_name = "Ilkka";
![img_7.png](image/img2-8.png)

###assignment 9
select distinct co2_budget from game;
![img_8.png](image/img2-9.png)

###assignment 10
select screen_name, co2_budget, co2_consumed, (@co2_left:=co2_budget-co2_consumed) as co2_left from game where screen_name = "Ilkka";
![img_9.png](image/img2-10.png)