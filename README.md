# Database
## ERD
ERD stands for entity relanshonship diagram and is used as a flowchart to show the relanshonship between diffrent entites. These entities could be people, objects or concepts. This type of flowchart is used to design databases using diffrent shapes to distinguish between diffrent types of enteties.
## ESD example
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/ERD.png)

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Insert
This command is used to insert values and data into tables.
INSERT INTO ENEMIES VALUES( 1, 50,'MAGE', 150,'HEALTHY' );
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Create
This command is used to create new tables with new values.

CREATE TABLE ENEMIES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, DAMAGE FLOAT NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE HEROES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, CLASS VARCJAR(50) NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE SPELLS( ID INT NOT NULL PRIMARY KEY, DAMAGEHEALING INT NOT NULL, NAME VARCHAR(50) NOT NULL, RANGE INT NOT NULL,
);

CREATE TABLE ENEMY_SKILLS( ENEMY_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);

CREATE TABLE HERO_SKILLS( HERO_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
Update
This command is used to update the value of data within a table without having to create a new table.

UPDATE HEROES SET LEVEL = 4 WHERE ID = 1;

UPDATE HEROES SET DAMAGE = 12.4 WHERE NAME = BOI;

UPDATE SPELLS SET RAGE = 4 WHERE ID = 4;

UPDATE SPELLS SET DAMAGEHEALING = 4 WHERE NAME = FIREBALL;
