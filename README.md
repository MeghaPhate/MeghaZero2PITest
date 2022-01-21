# MeghaZero2PITest
Demo Project


Table structure of player

create table PlayerDetails(
playerId int NOT NULL,
playerName varchar(20),
matchesPlayed int,
noOfMatchesWon int,
noOfMatchesLost int,
sportName varchar(20),
coachName varchar(20),
PRIMARY KEY(playerId)
);

1.Add player API call:
URL:http://localhost:3000/playerList
Method:POST
req example:
{
    
     "playerName" : "megha",
     "matchesPlayed" : 40,
     "noOfMatchesWon" :15,
     "noOfMatchesLost" : 25,
     "sportName" :"football",
     "coachName": "ninad"
}

2.Api call for Coach can get player List from database based on Player name and sport name;
URL:http://localhost:3000/playerList/:playerName/:sportName
Method:GET
req example:
playerName:megha
sportName:football

3:Api call for serach most efficient player is shown on top based on sport name
URL:http://localhost:3000/playerList/Search/efficientPlayer/:sportName
Method:GET
req example:
sportName : football

4:Api call for Admin can get all player list from  database;
URL:http://localhost:3000/playerList
Method:GET

