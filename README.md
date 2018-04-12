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
below is a table which contains diffrent features that were tested and completed during testing. This needs to be done to make sure that the database works when it is completed.

![Test Plan](https://github.com/HORNETJOE/Database/blob/master/table.PNG)

### Technical Documentation

#### General Information

#### System Overview

This database system is designed to hold information on different characters that appear in the game. It has different tables for Heroes, Enemies and other tables relating to skills that hold all of the key values relating to that character, including Name, ID, Health and Damage. These values can be updated in real time for gameplay purposes.

#### The Role Of Database Systems As…

Database systems can be used for a wide variety of things. The following is a list of different uses of database systems and what purpose they serve.

##### Back-end Systems
	
A Back-End Database is a database that can be accessed by different users through a third-party application rather than by application programming stored within the database itself or by manipulation of the data.
	
##### E-Commerce

In E-commerce, the main purpose of a database is to store information about the customer transactions, customer care, and inventory. By using a database,  programming a dynamic E-commerce website becomes easy as you only focus on the presentation and behavior of the website while all interactions are being managed by the system.

##### Data Mining Applications

Data mining is the process of discovering patterns in large data sets using different methods. It is an essential process where intelligent methods are applied to extract data patterns. During the process of data mining, the database(s) are searched for key information that could uncover new patterns or sequences in the data.


#### Tools Used

The following tools were used in the design and creation of the database system:

	-  draw.io 
	Used to create the Entity Relationship Diagram

	-  Microsoft Excel
	Used to create the data dictionary and the test plan documentation

	-  Microsoft Access
	Used to create the database system

 	-  Microsoft Word
	Used to create the user and technical documentation
