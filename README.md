# Database
## ERD
ERD stands for entity relanshonship diagram and is used as a flowchart to show the relanshonship between diffrent entites. These entities could be people, objects or concepts. This type of flowchart is used to design databases using diffrent shapes to distinguish between diffrent types of enteties.
## ESD example
![ERD flowchart](https://github.com/HORNETJOE/Database/blob/master/ERD.png)

/////////////////////////////////////////////////////////////////////////////////////////////////////

## User Stories

As a user I would like to be able to look up my heroes level

As a user I would like to be able to look up my enemies level

As a user I would like to be able to look up my heroes current health

As a user I would like to be able to look up my enemies current health

As a user I would like to see how much damage my spells do

As a user I would like to see the range of my different spells

As a user I would like to see how much damage the enemy does

As a user I would like to see the name of my enemies

As a user I would like to add new enemies using a form

As a user I would like to delete data entries using a form

As a user I would like to add new heroes using a form

As a user I would like to create a report

As a user I would like to use SQL code to add new tables to the database

The code below was used to create the database.

/////////////////////////////////////////////////////////////////////////////////////////////////////

## Data dictionary 
These are dictionaries which will help the viewer understand what type of input the table area will have, for example certain areas will have "text" next to them whereas others will have "float". This is to indecate whether there would be numbers or letters within the field of input. Data dictionaries are important as they can keep the database consistent from the start by giving it a set point as it allows viewers to look onto a clear view of what the database is going to be like and can always be referred back to when stuck.

/////////////////////////////////////////////////////////////////////////////////////////////////////
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

### What Is an Object Oriented Database?

An object database is a database system in which data is represented in the form of objects similar in design to object oriented programming. Object databases are different from relational database which are table-oriented. Object-relational databases are a mix of both approaches.

Object-oriented database management systems combine database capabilities with object oriented programming language capabilities. This design allows object-oriented programmers to develop the product, store them as objects, and duplicate and edit existing objects to make new objects Because the database is connected with the programming language, the programmer can maintain a high level of consistency, in that both the OODBMS and the programming language will use the same model to represent themselves. Relational database management system projects maintain a clearer division between the database model and the application.

### What Is the System for?

The system is designed to hold data on the status of different characters and spells within the game, this system will help the game be able to hold multiple bits of data in order to complete its task.

## Risks/contingencies

### Risks

The risks of this database are in the design and development stage, a few possible risks for this database are:
Database not updating reports from forms and having the data stay the same,
The forms having different characters and integers entered within them that they are programmed for.
The tables not communicating with each other and not updating with each other,
Having any of the forms not show the information that the tables have,

### Contingencies

The risks can be managed by planning constancies in order to help risks be prevented, some of the contingencies that we used were:
Keeping multiple saves in case a change ruined the database,
Having an ERD so that the database would keep to a specific design,
Keeping code saved in order to inspect it if anything went wrong,
Testing every bit of code after it was executed to make sure it all worked well,

### Design Decisions

The design of the database was decided when planning the database, we used ERD’s to plan and figure out what would be best for the database, this also meant that we could test to make sure the tables connecting with each other would work well when running together.
Making the ERD’s required planning on how the database worked, we looked at the requirements of the database and the functionality on it, this included how it would work, what it would be used for and why is it being made, looking at these questions allowed us to create a template that would suite all of the needs that needed to be addressed within the database.

### Key Factors Influencing Design

The key factors for the design was the functionality of the database, since it was being made for a game to hold data on the characters and their skills, it meant that designing it would have to revolve around that, keeping to this meant that we were able to keep a key design in mind.

### Functional Design Decisions

Being made for a game, it meant that the functionality must cater for the game’s needs, for example the database was made to hold data on heroes, villains and their skills that they had, so for this it meant that all parts of it needed to be addressed. The database was able to function at a point where it could hold all the data and be able to change it in order to keep the game running well.

### Database Management System Decisions

The database was managed by Microsoft access, we used this software as it allowed us to use all the tools we needed in order to create the database as we wanted to, this included having SQL queries integrated within it, allowing a design document as well as forms allowing for real time updating for reports. Having these tools allowed us to create a successful website that fulfilled the requirements for our game.

### Security and Privacy Design Decisions

The database is a private database, this means that the only people that can access it are the people that are on the file that it is created on, this means that only the creator and anyone that they want to share it with have access to the database. This means that there cannot be any breaches of the data at this point in time.

### Performance and Maintenance Design Decisions

The database is not big and has few requirements, the scope of the project was not big, this meant that performance wise the database is extremely quickly and maintenance is not difficult. The database had no need to be any bigger than it was, this meant that from the design stage, there was no need to make big decisions on the performance of the database.

### Detailed Database Design

The database was made in order to cater for a game, for this we made 5 tables, having five meant that we could cover all the aspects of the database’s function, whilst also keeping it performance light and also keeping the maintenance low. The five tables were Heroes, Villains, Heroes_Skills, Villains_Skills and Skills, these were enough in order to cover all points of the database. The forms of the database make sure that the data that is stored on their is clear and has a place to update the reports more. The reports that are included are made in order for people to view the data currently stored in the tables, this data will update in real time from when the forms are changed.

### Data Software Objects and Resultant Data Structures

For the forms, we have created buttons that allow the viewer to change the data that is stored within the tables, these allow the data to be updated from the forms easily, as well as this there is a delete or remove button that can also be used in order to remove part of the database. The data is structured so that the data can be updated and edited from anywhere other than the reports, this means that the reports are easier to see and collect information from and can be focused on viewing the data rather than editing it.

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
