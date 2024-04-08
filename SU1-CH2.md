# SU1-CH2
2024-04-08 | 23:09
{Subject}:[[CMPG 311]]
{Section}:[[Chapter 1 - Database Systems]]
{Tags}: #Databases 
{Related}: #Programming 

--- 
### The Internal Model

Representing database as seen by the DBMS mapping conceptual model to the DBMS
- Internal schema: specific representation of an internal model, using the database constructs supported by the chosen database
- Logical independence: changing internal model without affecting the conceptual model
- Hardware independent: unaffected by the type of computer on which the software is installed
---
### The Physical Model

Operates at lowest level of abstraction
- Describes the way data are saved on storage media such as magnetic, solid state, or optical media
Requires the definition of physical storage and data access methods
- Software and hardware dependent

Relational model aimed at logical level
- Does not require physical-level details

Physical independence: changes in physical model do not affect internal model

---
$$
\begin{array}{l|l|l|l}
\hline \begin{array}{l}
\text { Table 2.4 } \\
\text { Levels of Data } \\
\text { Abstraction }
\end{array} & & & \\
\hline \text { Model } & \begin{array}{l}
\text { Degree of } \\
\text { Abstraction }
\end{array} & \text { Focus } & \text { Independent of } \\
\hline \text { External } & \text { High } & \text { End-user views } & \begin{array}{l}
\text { Hardware and } \\
\text { software }
\end{array} \\
\hline \text { Conceptual } & \text { Medium-High } & \begin{array}{l}
\text { Global view of data } \\
\text { (database model } \\
\text { independent) }
\end{array} & \begin{array}{l}
\text { Hardware and } \\
\text { software }
\end{array} \\
\hline \text { Internal } & \text { Medium-Low } & \begin{array}{l}
\text { Specific database } \\
\text { model }
\end{array} & \text { Hardware } \\
\hline \text { Physical } & \text { Low } & \begin{array}{l}
\text { Storage and } \\
\text { access methods }
\end{array} & \begin{array}{l}
\text { Neither hardware nor } \\
\text { software }
\end{array} \\
\hline
\end{array}
$$
--- 
{Efundi Lecture Notes}: [SU1-CH2]()