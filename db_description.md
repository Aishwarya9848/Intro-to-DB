Group: 15

Database Description:

|Table|Attributes|Primary Key|Foreign Key|3NF|
| :- | :- | :- | :- | :- |
|Players|<p>Player\_ID, First\_Name,</p><p>Last\_Name,</p><p>Team\_ID</p>|Player\_ID|Team\_ID|Yes|
|Teams|<p>Team\_ID,</p><p>Team\_Name,</p><p>Match\_ID,</p><p>Match\_Points</p>|Team\_ID|Match\_ID|Yes|
|Matches|<p>Match\_ID,</p><p>Match\_Name,</p><p>Match\_Location</p><p>Tournament\_ID</p>|Match\_ID|Tournament\_ID|Yes|
|Tournaments|<p>Tornament\_ID,</p><p>Tournament\_Name,</p><p>Tournament\_Level,</p><p>Prize</p>|Tournament\_ID||Yes|

Functional Dependencies:

Table: Players

Player\_ID -> First\_Name

Player\_ID-> Last\_Name

Player\_ID->Team\_ID

Table: Teams

Team\_ID->Team\_Name

Team\_ID -> Match\_ID

Team\_ID -> Match\_Points

Table: Matches

Match\_ID-> Match\_Name

Match\_ID-> Match\_Location

Match\_ID-> Tournament\_ID

Table: Tournaments

Tournament\_ID -> Tournament\_Name

Tournament\_ID->Tournament\_Level 

Tournament\_ID ->Prize

We have created four tables in our database and named them as Players, Teams, Matches, Tournaments. Primary keys respectively for the above tables are Player\_ID, Team\_ID, Match\_ID, Tournament\_ID. Foreign keys for the tables Players, Teams, Matches are Team\_ID, Match\_ID, Tournament\_ID respectively. 


Tables and sample data:

Table Name: Players

|Player\_ID|First\_Name|Last\_Name|Team\_ID|
| :- | :- | :- | :- |
|1|Virat|Kohli|1|
|2|Rohit|Sharma|1|
|3|Joe|Root|3|
|4|David|Warner|2|
|5|Aaron|Finch|2|
|6|Kane|Williamson|6|
|7|Tamim|Iqbal|5|
|8|Nicholas|Pooran|8|
|9|Dale|Steyn|4|
|10|Kumar|Sangakkara|7|
|11|Babar|Azam|9|
|12|Mahela|Jayewardene|7|



Table Name: Teams

|Team\_ID|Team\_Name|Match\_ID|Match\_Points|
| :- | :- | :- | :- |
|1|India|1|2|
|2|Australia|1|0|
|3|England|2|2|
|4|South Africa|2|0|
|5|Bangladesh|3|1|
|6|New Zealand|3|1|
|7|Sri Lanka|4|2|
|8|West Indies|4|0|
|9|Pakistan|5|0|




Table Name: Matches


|Match\_ID|M\_Name|Match\_location|Tournament\_ID|
| :- | :- | :- | :- |
|1|Match1|Hyderabad|1|
|2|Match2|Bangalore|1|
|3|M3|Sydney|2|
|4|M4|Melbourne|2|
|5|Match3|Mumbai|1|
|6|M1|London|3|



Table Name: Tournaments


|Tournament\_ID|Tournament\_Name|Tournament\_Level|Prize|
| :- | :- | :- | :- |
|1|World Cup|Multi Nation|$800000|
|2|Champions Trophy|8 teams|$500000|
|3|Bilateral|2 teams|$100000|
|4|Triangular|3 teams|$300000|
|5|World Test Championship|5 teams|$400000|


