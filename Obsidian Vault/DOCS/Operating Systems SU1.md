# SU1
2024-07-20 | 14:35
{Subject}: [[CMPG 324]]
{Section}: [[SU1]]
{Tags}: #OperatingSystems #Programming #ComputerScience
{Related}: #Databases #Java 

--- 
Know the different modes that programs have.
- User mode - Programs in this mode cannot access unauthorized data and hardware, they can only present requests to the kernel and the kernel will allocate the required resources. 
- Kernel mode - Kernel mode has full access to systems hardware and programs. Full control and management of file systems data and components.

For a user program to gain access to resources the program must create a system request that the kernel will evaluate and provide the needed resources if it is available.

### Primary Functions of an Operating System
- Provide a clean abstraction of System Resources to system users.
- Manage those resources in a safe and efficient way.   
#### Architecture
The Architecture of most systems are primitive and awkward and it is the job of the OS to reduce the complexity and give a simple method to interact.

#### Drivers
A Driver is effectively an interface that allows for a device to be used with simple instructions such as read and write, rather than the massive number of instructions that would be needed otherwise.

#### Multiplexing 
Without a way to effectively manage resources there would be chaos. Multiplexing manages this task.

### Resource Management
The management of resources are separated into three primary levels:
- Process Control: which effects every single process and instruction run on the machine;
- Input and Output Control: which comes into play whenever data is transferred between devices;
- Memory Management and the File System, Deals with both primary memory and secondary memory.

### Types of Operating Systems
- Mainframe operating systems
- Server operating systems
- Multiprocessor operating systems
- Personal Computer operating systems
- Handheld Computer operating systems
- Embedded operating systems
- Sensor-Node operating systems
- Real-Time operating systems
- Smart Card operating systems

### After successful completion of this study unit, you should be able to:
- describe the various levels that make up a computer system;
- discuss microprogramming;
- discuss the two functions performed by an operating system;
- discuss the core concepts that developed in the history of operating systems;
- discuss the core concepts of processes and files; and
- describe the general operation of system calls.

## History of Operating Systems and Computers
#### The First Generation
Period : 1945 - 1955
The computers from this period used vacuum tubes for transistors, these computers had no software in the modern sense. these computers were usually hardwired. By the 1950s however they developed punch cards to do the "Programming".
#### The Second Generation
This Generation was when transistors were implemented using semi-conductors. The computers developed in these days were called mainframes. This brought improvements in power consumption and production costs, leading to them being sold to customers and making builders and programmers discrete groups of individuals. Punch cards were still used and programming was done on paper before they were punched. This generation also introduced the first "Pre-processing", or batch, systems, where a less powerful machine would be used to help optimize the processing time of more powerful machines buy creating a large series of operations that could be run consecutively (the "Batch"). The control program that the mainframe used to load the operations is considered a precursor to modern operating systems. Eventually these second generation machines started running operating systems such as FMS (Fortran Monitoring System) and IBMSYS
#### The Third Generation
Here we have the introduction of integrated circuits (or IC) powered machines that all had the same architecture. Meaning that in theory that any piece of IBM compatible software could run on any IBM machine. This was attempted using a highly complex operating system. With this new operating system came feature still used such as multiprogramming and spooling. This generation also introduced the "Server-Client" model for timesharing, where a mainframe's resources would be shared amongst users by use of networked terminals. This lead to the development of minicomputers, and in turn, small single user operating systems such as Unix.
#### The Fourth Generation
Due to the development of precision manufacturing equipment, thousands of transistors could be placed in a small space in the early 1980s. This birthed the generation still used today, MS-DOS, and eventually Windows.
#### The Fifth Generation
The primary distinction between the fourth and fifth generation is the involvement of mobile computers.

--- 
## The CPU
[[The CPU]]






--- 
{Efundi Lecture Notes}: [Advanced Databases SU1]()