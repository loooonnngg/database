#week 5

###assignment 1
update game
set  location = (select ident from airport where name = "Nottingham Airport"), co2_consumed = co2_consumed+500
where screen_name = "Vesa";
select * from game;
![img.png](image/img7-1.png)

###assignment 3
delete from goal_reached;
select * from goal_reached;
![img.png](image/img7-3.png)

###assignment 4
delete from game;
select * from game
![img.png](image/img7-4.png)