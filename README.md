# Database
## ERD
ERD stands for entity relanshonship diagram and is used as a flowchart to show the relanshonship between diffrent entites. These entities could be people, objects or concepts. This type of flowchart is used to design databases using diffrent shapes to distinguish between diffrent types of enteties.
## ESD example
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/ERD.png)

/////////////////////////////////////////////////////////////////////////////////////////////////////

The code below was used to create the database.

#### Insert

INSERT INTO ENEMIES VALUES( 1, 50,'MAGE', 150,'HEALTHY' );

/////////////////////////////////////////////////////////////////////////////////////////////////////

#### Create

CREATE TABLE ENEMIES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, DAMAGE FLOAT NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE HEROES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, CLASS VARCJAR(50) NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE SPELLS( ID INT NOT NULL PRIMARY KEY, DAMAGEHEALING INT NOT NULL, NAME VARCHAR(50) NOT NULL, RANGE INT NOT NULL,
);

CREATE TABLE ENEMY_SKILLS( ENEMY_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);

CREATE TABLE HERO_SKILLS( HERO_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);

/////////////////////////////////////////////////////////////////////////////////////////////////////

#### Update

UPDATE HEROES SET LEVEL = 4 WHERE ID = 1;

UPDATE HEROES SET DAMAGE = 12.4 WHERE NAME = BOI;

UPDATE SPELLS SET RAGE = 4 WHERE ID = 4;

UPDATE SPELLS SET DAMAGEHEALING = 4 WHERE NAME = FIREBALL;

/////////////////////////////////////////////////////////////////////////////////////////////////////

#### Developing the database
below are images display the database and its diffrent functions displays.

![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/database%20image%20heros.PNG)

#### output
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/interface.PNG)

#### input
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/input.PNG)

#### query
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/query.PNG)

#### Testing
![Test Plan](https://github.com/LukeShead/Databases/blob/master/Test%20plan.JPG)
