create table Players(

Player\_ID int(10) NOT NULL PRIMARY KEY, 

First\_Name varchar(10), 

Last\_Name varchar(10), 

Team\_ID int(10), FOREIGN KEY (Team\_ID) references Teams(Team\_ID)

);


create table Teams(

Team\_ID int(10) NOT NULL PRIMARY KEY,

Team\_Name varchar(50), 

Match\_ID int(10), FOREIGN KEY(Match\_ID) references Matches(Match\_ID)

Match\_Points int(10),

);


create table Matches(

Match\_ID int(10) NOT NULL PRIMARY KEY, 

Match\_Name varchar(50), 

Match\_Location varchar(50), 

Tournament\_ID int(10), FOREIGN KEY (Tournament\_ID) references Tournament(Tournament\_ID)

);


create table Tournaments(

Tournament\_ID int(10) NOT NULL PRIMARY KEY, 

Tournament\_Name varchar(50), 

Tournament\_Level varchar(10), 

Tournament\_Prize double)

);

