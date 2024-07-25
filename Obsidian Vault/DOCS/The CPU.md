# The CPU
2024-07-20 | 20:15
{Subject}:[[CMPG 324]]
{Section}:[[SU1]]
{Tags}: #Programming #ComputerScience #OperatingSystems 
{Related}: [[CMPG 311]] [[CMPG 313]] [[CMPG 211]] 

--- 
### The CPU
The CPU, or Central Processing Unit, of a computer is responsible for executing commands, and therefore processing data. 
There are many variations in CPU Architectures and instruction sets and this requires specially written operating systems

---
### Registers
This is the fastest memory in a computer and are located on the CPU. They are extremely fast and expensive so small amounts are used.

- Registers: each CPU has a number of registers to hold key values or temporary results to improve processing speed. There are also a number of special registers, such as the
- **program counter**, which contains the memory address of the next instruction to be fetched from memory;
- **stack pointer**, which points to the top of the memory stack. This stack hold information about procedures that have been started, but have not yet exited(i.e. procedures that are still "running"); and
- **Program Status Word (PSW)**, which contains control bits that are mostly used by system calls and Input/Output (I/O) operations.
---
- Mode: Most CPUs have a kernel mode and a user mode.
### Threading 
- Threading: CPUs may support multithreading, which allows for multiple processes to run concurrently. This means the CPU can switch quickly between multiple instruction threads.
### Cores 
While Threading cannot offer true concurrent processing, having multiple cores (CPU's) can. A CPU in modern systems have multiple Cores.
### Cache
CPU cache is very small very high speed and very expensive memory units that holds the instruction before they are processed such as a clip of ammunition in a gun. This is the L1 cache. 
Some CPUs also have a second memory unit, called the **L2 cache**, that is used to store recently used data.

--- 
{Efundi Lecture Notes}: [The CPU]()