**Operations on Players table**

UPDATE Players

SET Player\_Id = 6 

WHERE First\_Name= ‘Virat’;

Select \* from players where Player\_id = 6

DELETE FROM Players WHERE Player\_id = 1 OR Player\_Id = 6;

Select \* from players where Player\_id = 1 OR Player\_id = 6

SELECT First\_Name, Last\_Name

FROM Players

WHERE Team\_ID IN (

`    `SELECT Team\_Name

`    `FROM Teams

);


**Operations on Teams table**

UPDATE Teams

SET Match\_points = 10 

WHERE Team\_id= 1;

Select \* from Teams where Team\_id = 1

DELETE FROM Teams WHERE Team\_id = 4;

Select \* from Teams where Team\_id = 1 OR Team\_id = 4

SELECT Team\_Name

FROM Teams

WHERE Match\_ID IN (

`    `SELECT Match\_Name

`    `FROM Matches

);




**Operations on Matches table**

UPDATE Matches

SET Match\_Name = ‘WSU’

WHERE Tournament\_ID= 1;

Select \* from Matches where Tournament\_ID= 1;

DELETE FROM Matches WHERE Match\_Name = ‘M4’

Select \* from Matches where Tournament\_ID= 1OR Match\_Name = ‘WSU’


SELECT Match\_Name

FROM Matches

WHERE Tournament\_ID IN (

`    `SELECT Tournament\_Name

`    `FROM Tournament


**Operations on Tournaments table**

UPDATE Tournaments

SET Prize= ‘$190000’

WHERE Tournament\_ID= 1;

Select \* from Tournaments where Tournament\_ID= 1;

DELETE FROM Tournaments WHERE Tournaments \_Name = ‘Triangular’

Select \* from Tournamnets where Tournament\_ID= 4 OR Tournaments \_Name = ‘Triangular’
