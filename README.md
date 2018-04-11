# Database
## ERD
ERD stands for entity relanshonship diagram and is used as a flowchart to show the relanshonship between diffrent entites. These entities could be people, objects or concepts. This type of flowchart is used to design databases using diffrent shapes to distinguish between diffrent types of enteties.
## ESD example
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/ERD.png)

INSERT INTO ENEMIES VALUES( 1, 50,'MAGE', 150,'HEALTHY' );

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

This command is used to create new tables with new values.

CREATE TABLE ENEMIES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, DAMAGE FLOAT NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE HEROES( ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL, NAME VARCHAR(50) NOT NULL, CLASS VARCJAR(50) NOT NULL, HP FLOAT NOT NULL );

CREATE TABLE SPELLS( ID INT NOT NULL PRIMARY KEY, DAMAGEHEALING INT NOT NULL, NAME VARCHAR(50) NOT NULL, RANGE INT NOT NULL,
);

CREATE TABLE ENEMY_SKILLS( ENEMY_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);

CREATE TABLE HERO_SKILLS( HERO_ID INT NOT NULL PRIMARY KEY, SPELL_ID INT NOT NULL PRIMARY KEY, LEVEL INT NOT NULL,
);
