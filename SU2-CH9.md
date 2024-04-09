# SU2-CH9
2024-04-09 | 18:22
{Subject}:[[CMPG 311]]
{Section}:[[]]
{Tags}: #Databases 
{Related}:

--- 
#### The Information System

 The database is part of a larger whole known as an information system (IS)
- Provides for data collection, storage, and retrieval
- People, hardware, and software
- Database(s), application programs, and procedures

 Systems analysis: establishes need for and extent of information system
- Systems development: process of creating information system

Performance factors of an information system
- Database design and implementation
- Application design and implementation
- Administrative procedures

Database development
- Process of database design and its implementation

---
Systems Development Life Cycle (SDLC)

Traces history of an information system
- Provides a picture within which database design and application development are mapped out and evaluated

Traditional SDLC is divided into five phases
- **Planning**: yields a general overview of the company and its objectives
- **Analysis**: problems defined during planning phase are examined in greater detail
- **Detailed systems design**: designer completes the design of the system's processes
- **Implementation**: hardware, DBMS software, and application programs are installed, and the database design is implemented
- **Maintenance**: corrective, adaptive, and perfective

Iterative rather than sequential process

---
#### Computer-Aided Systems Engineering (CASE)

- =Tools used to automate part or all of the SDLC
- Includes System Architect and Visio Professional
- Helps produce better systems in a reasonable amount of time and reasonable cost

Applications are more structured, better documented and standardized
- Prolongs operational life of systems
- Easier and cheaper to update and maintain
---
#### The Database Life Cycle

The Database Life Cycle (DBLC) contains six phases

- **Database initial study**: define problems, constraints, objectives, scope, and boundaries
- **Database design**: making sure that the final product meets user and system requirements
- **Implementation and loading**: DBMS is installed, database is created, and data is loaded or converted

**Testing and evaluation**: database is tested, fine-tuned, and evaluated

	- Full backup/dump: all database objects are backed up in their entirety
	- Differential backup: only modified/updated objects since last full backup are backed up
	- Transaction log backup: only the transaction log operations that are not reflected in a previous backup are backed up

- **Operation**: problems are identified and solutions implemented
- **Maintenance and evolution**: preventative, corrective, adaptive, etc.

---
$$
\begin{aligned}
&\text { Purpose of Database Initial Study }\\
&\begin{array}{||c||c||}
\hline \begin{array}{c}
\text { Analyze } \\
\text { company } \\
\text { situation }
\end{array} & \begin{array}{l}
\text { Define problems } \\
\text { and constraints }
\end{array} \\
\hline \begin{array}{c}
\text { Define } \\
\text { objectives }
\end{array} & \begin{array}{c}
\text { Define scope } \\
\text { and boundaries }
\end{array} \\
\hline
\end{array}
\end{aligned}
$$
---
### Description of Operations

- Provides precise, up-to-date, and reviewed description of activities defining an organization's operating environment
- Business rules are derived from a Description of Operations

---
Database Design
- Supports company's operations and objectives
- Most critical phase
	- Ensures final product meets user and system requirements
- Points for examining completion of Design phase procedures
	- Data component is one element of information system
	- System analysts/programmers design procedures to convert data into information
	- Database design is an iterative process
---
---

# Conceptual Design 

- Goal: design a database independent of database software and physical details
	- Conceptual data model: describes main data entities, attributes, relationships, and constrains
		- Designed as software and hardware independent


**Minimum data rule**
- All that is needed is there, and all that is there is needed

---
$$
\begin{array}{|l|l|}
\hline & \text { Table 9.2: Conceptual Design Steps } \\
\hline \text { Step } & \text { Activity } \\
\hline 1 & \text { Data analysis and requirements } \\
\hline 2 & \text { Entity relationship modeling and normalization } \\
\hline 3 & \text { Data model verification } \\
\hline 4 & \text { Distributed database design } \\
\hline
\end{array}
$$

---
#### Data analysis and requirements

Designers efforts are focused on 
- Information needs, users, sources and constitution

Answers obtained from a variety of sources
- Developing and gathering end-user data views
- Directly observing current system: existing and desired output
- Interfacing with the systems design group

Entity relationship modeling and normalization
- All objects (entities, attributes, relations, views, and so on) are defined in a data dictionary, which is used in tandem with the normalization process

---
--- 
{Efundi Lecture Notes}: [SU2-CH9](https://1drv.ms/b/s!AlwTrhPAanGFhPg6Ysydlu042kCa1g?e=RVKooG)
<iframe src="https://onedrive.live.com/embed?resid=85716AC013AE135C%2180954&authkey=!AFFfm7Aa_pgvSwI&em=2" width="800" height="600" frameborder="2" scrolling="yes"></iframe>