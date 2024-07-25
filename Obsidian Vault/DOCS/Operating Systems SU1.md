# SU1
2024-07-20 | 14:35
{Subject}: [[CMPG 324]]
{Section}: [[SU1]]
{Tags}: #OperatingSystems #Programming #ComputerScience
{Related}: #Databases #Java 

--- 
Know the different modes that programs have.
- User mode - Programs in this mode cannot access unauthorized data and hardware, they can only present requests to the kernel and the kernel will allocate the required resources. 
- Kernel mode - Kernel mode has full access to systems hardware and programs. Full control and management of file systems data and components as well as memory management.

For a user program to gain access to resources the program must create a system request (**System Call**) that the kernel will evaluate and provide the needed resources if it is available.

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

![[KBpm7EzHod6Pk2mmkPSTSz1Y1EShzFqwpNehpDwUUuI.original.fullsize.png]]
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
### RAM
Then we have the RAM this is where data is stored before being taken into the cache (L1 cache) its like having ammunition clips ready for after the one in the gun is processed and is slower process to move the clip into the gun. Plainly the ram is slower than the cache.

### Secondary Memory
Then comes "secondary memory", such as disks. Stores data even if the computer looses power. Long term memory.
### I/O Devices
I/O devices, simply stated, are responsible for handling the flow if information between devices such as hard drives and memory
### Buses
**Buses** are "microsystems" that manage the transfer of data between the various components of a computer.
- The memory bus is responsible for transferring data between the CPU, memory and peripherals.
---
The **chipset**, which is usually a part of the motherboard, is a set of components that manage the flow of information between the CPU, memory, and peripherals.
### Direct Media Interface (DMI)
**Direct Media Interface (DMI)** bus deserves mention. The DMI is used to allow for a system to separate the slower devices, such as device controllers, from the faster devices, such as the CPU and memory.

 The **northbridge** chip is used to connect the CPU, memory, and **Peripheral Component Interconnect Express (PCIe)** bus with one another, and is therefore also called the **memory controller hub**.

The northbridge is connected directly to the CPU by means of the **Front-Side Bus (FSB)**.

The slower devices, such as the device controllers, are connected to the **southbridge**. Because the southbridge is mainly connected to I/O devices, it is called the **I/O Controller Hub (ICH)** in Intel systems (AMD calls their southbridge the **Fusion Controller Hub (FCH)**).

### Interupts
An interrupt, simply put, is a message from a device or a controller that lets a higher device know that it is done with the work that was assigned to it.

If a program wants to read a small file, for example, the CPU will send a command to the relevant device controller, which will in turn tell the drive to start reading data. Once the drive has finished reading the requested data, it lets the controller know by sending an interrupt. Once the controller is in a position to handle the interrupt, it in turn sends an interrupt to the CPU to let it know that the job is done. The CPU can then accept the data as soon as it is ready to do so.

---
**Processes**: A process is, quite simply, a program or piece of code that is being executed. Each process has its own **address space**, which is the section of memory that has been allocated to and reserved for that process.

**Files:** Files are specific abstractions of binary data stored on secondary memory devices

**Protection/security**: In addition to operating protections, such as those that prevent processes from accessing other processes' address space, an OS also has to protect the data and resources of the user

**Systems calls**: a system call, simply stated, is a request by a process for the OS to execute some code that may require kernel access.

**Microprogramming**: microprogramming allows for a CPU to have an instruction set, rather than a set number of hardwired functions.

### System Calls
An example of the read system call is shown in the figure below, which also illustrates how much the operating systems does to simply common tasks:

![[Z4tOKAXP4_vZXo_-6Cv3ubo1Wa_ACxdkrSrAX1FMh4g.original.fullsize.png]]
### Different OS Structure Configurations
- **Monolithic**: the entire OS runs as a single program in kernel mode
- **Layered**: the OS is divided into multiple layers, with each layer being responsible for a specific kind of task. The higher layers then build on the functions provided by the lower layers.
- **Microkernels**: the OS is split into two main parts: that which does not require kernel access, and as small a part as possible that does. Only a small part of the OS therefore runs in kernel mode.
- **Client-server**: all OS processes are split into two groups, namely the servers that provide services, and the clients that use those services. This allows for an OS to potentially be split amongst machines of varying capability, but this is not a requirement.
- **Virtual machines**: the virtual machine OS structure allows for multiple operating systems to run on the same hardware.
- **Exokernels**: with an exokernel structure, the hardware is partitioned amongst the users. If it were to be compared to the virtual machine structure, then all of the virtual machines have access to all of the hardware, whereas exokernel systems would only have access to a part of the system.


--- 
{Efundi Lecture Notes}: [Advanced Databases SU1]()