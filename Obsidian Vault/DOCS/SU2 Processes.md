# SU2 Processes
2024-07-25 | 20:41
{Subject}:[[CMPG 324]]
{Section}:[[SU2 Processes]]
{Tags}: #OperatingSystems #Programming #ComputerScience 
{Related}:

--- 
### Processes
A **process** is, quite simply, an abstraction of a running program.
 - It is also important to note that each instance of a program is a different process
 - a program has to be running in order for there to be a process of that program.

### Process Model
In the **Process Model**, which deals with these concepts, all of the software (sometimes including the OS) running on a computer is organized into collections of so-called **sequential processes** or just **process**. Each process is a unique instance of a running program, and contains the values of all the variables, program counter values, and register values. Each process acts as if it has exclusive access to the CPU but, in reality, the CPU rapidly switches between the various processes in order to complete all of the instructions associated with all of them.

### Multiprogramming
This situation, whereby a CPU rapidly switches between multiple processes, is called **multiprogramming**. 
For example a university student in a semester has multiple modules to complete. One could argue that this is a form of academic **pseudoparallelism**, as all of these significant tasks are done simultaneously, but each task gets the student's full attention for only a brief amount of time, before another task then gets attention.

---
- A **beginning** (**input**);
- An **end** (**output**);
- A transition point somewhere between the beginning and the end (**a state**); and
- An overarching action (**a program**).

In order to **create** a process, one of four things usually has to happen:

- System initialisation;
- A running process makes a process-creation system call;
- A user requests the creation of a new process; or
- A batch job is initiated.

---
### Processes Hierarchy and Child Processes
In some operating systems, the OS keeps track of which processes started which processes. When a process is started by another one, it is considered a child of the creating process. This means that a process hierarchy can be formed, and also that entire collections of processes can be monitored. This is particularly useful if you have some kind of program that needs another program to do something. If the parent process stops working for whatever reason, there is no longer any reason for the child to continue, and all of the processes in the hierarchy can be stopped. As a result, you don't have to go hunting for errant processes that waste resources when something goes wrong with the parent process.

---

### Termination of Processes
Naturally, all processes have an end, which requires their **termination**. A process usually ends as a result of one of 4 events:

- **Normal exit**, which is a voluntary termination that occurs when a process finishes its work without issues, or if the user decides to end it (click the red cross, so to speak);
- **Error exit**, which is also a voluntary termination. An Error exit occurs when a process encounters an error caused by external factors, such as a user inputting bad data, and decides to stop;
- **Fatal exit** is an involuntary termination that occurs when a process encounters an unresolvable error caused by it's own code (think unhandled exceptions - these would cause fatal exits); and
- A process can also be involuntarily **killed by another process**.

---
### Process States
All processes have a specific **state** that describes their current situation. There are 3 states that a process can have, specifically:

- **Running**, which means that process is actually using the CPU at that very moment;
- **Ready**, which means that the process is ready to use the CPU, but has been stopped for some reason (such as to give another process a go); and
- **Blocked**, in which case the process will be prohibited from using the CPU until some external event happens (external meaning outside the blocked process).

There is a limit to how these processes can change between states

![[yUT_Oz8x7brgvr3Qxi1k2qvHk_rgRTkHePgbgiSVea4.original.fullsize.png]]
--- 
{Efundi Lecture Notes}: [SU2 Processes]()