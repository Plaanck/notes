# Operating Systems

- The operating system is a platform for the software of a computer to be able to communicate with the hardware.
- For example, one feature that modern operating systems have is ***Multitasking***
	- Multitasking is where you can have more that one program running at the same time. 
	- What a single core multitasking system does, is allocate a small amount of time to each process, and switch between them at a speed that we don't notice the gaps in-between.

- Another example is File handling, 
	- The OS can present your files in an organised structure, with names, and showing you the extensions of your files, as well as allowing you to rename and move them.

- Another example is User Management
	- This allows many users to log into the same computer.
	- The OS will be able to retain settings for each user, and have different access rights to files and programs.

- A big feature of GUI style OS's is WIMP, meaning
	- Windows
	- Icons
	- Menus
	- Pointers
- This the most common style of modern Operating Systems, but other styles include:
	- Command Line Interface: No menus or pointers, just a command prompt
	- Menu Interface: Shows menus, which allow you to select the different options, but still no pointer or icons etc.


# Memory Management

- There are two types of memory management
	- **Segmentation** - The memory blocks that are allocated to processes are divided into **segments** of **different sizes** to fit the varying memory requirements of each process. The segments do not need to be stored continuously across a fixed address space, and they can be moved in and out of memory as required.

	- **Paging** - The logical address space is divided into memory units called **pages**. When a page is loaded into the main memory, it is stored in a **page frame**, which is a block of sequential addresses that is the same size (has the same number of addresses) as a page. Pages of the same process do not need to be stored together, but can be allocated wherever there is free space in the main memory. A **page table** is used to keep track of which page frame is allocated to each page.



## Virtual Memory

- When too many programs are open, or there is lots of heavy processing, we can run out of RAM, meaning we shouldn't be able to load anything else. 
- However, we can use Virtual Memory (not to be confused with [[3.4 - Virtual Storage||Virtual Storage]])
	- Virtual Memory takes advantage of the larger capacity of secondary storage, it can take up an allocated amount of the secondary storage, and use it in place of RAM.
	- The OS can switch processes from RAM and Virtual Memory, when needed
	- The issue with this is that virtual memory is a lot slower than RAM, as it was intended for non volatile storage, but when needed it is effective as a substitute when out of RAM.

# Interrupts and Scheduling

- Scheduling is a necessary part of **Multitasking**,
- The Scheduler is the system that organizes which process gets what amount of time and when.
- The **process ready queue** is where the processes are lined up to be processed, and functions the same as a [[3- Queues|Queue Data Structure]] 
- From the ready queue the CPU runs the process for a set amount of time e.g. 5 ticks.
	- From the CPU, the process may be finished, and no longer need to be put back into the queue.
	- Or, the process either gets blocked from being put back into the queue due to the fact that it requires an I/O to continue.
	- Alternatively, the process runs for its set amount of time (time slice / quantum), and is still not finished, so it is sent to the back of the queue.
- The processes do not necessarily have to follow the FILO structure of conventional queues, the behavior of the items in the queue can be changed according to the **Scheduling Algorithm** 

## Scheduling Algorithms

- First Come First Serve (FCFS)
	- This following the default FILO structure of a queue
	- Complete processes in the order they enter the queue

- Shortest Job First (SJF)
	- Picks the process that takes the shortest amount of time and runs them until they finish

- Round Robin (RR)
	- Each process is allocated a fixed amount of time (Time Slice / Quantum)
	- If the process is not completed by the end of the time slice it returns to the end of the queue

- Shortest Remaining Time (SRT)
	- Similar to Shortest Job First, but it is a **pre-emptive algorithm**
	- This means that processes can be suspended if a higher priority process joins the queue
	- So a process could run through its quantum, and no longer be the shortest remaining time, and swap.

## Process Blocking

 - A process may begin to be ran, but require data from the HDD
 - The HDD is slow compared to the CPU, so we can "block" A, and remove it from the queue, to wait until the data required is received.
 - An interrupt is a signal that is sent from a program to tell the CPU that the process is to be added back to the queue.

## Multi-Level Feedback Queues (MLFQ)

- In a computer with more than just one core, then we can have multiple process ready queues.
- With a MLFQ, different queues can have different priorities, e.g. different Scheduling Algorithms


# Types of Operating Systems


- Multitasking OS
	- With general purpose systems, such as phones, computers, we need to be able to run more than one application at the same time, e.g. listening to music while writing on a word document, as the clock shows the time updating, and the antivirus checks for vulnerabilities.
	- Each active program is allocated a small time slice of processing 

- Multi-user OS
	- An operating system that allows multiple people to use a computer at the same time, commonly found in schools or work.
	- The OS manages the user's access levels and security clearance when they log on.
	- Server OS will handle the requests of multiple users using different computers at the same time.

- Distributed OS
	- In a distributed computing, the OS controls and coordinates the computers across a network, presenting them to the user as if it were a single system
	- For example, Online shopping sites may use this technique, your basket could be handled by one machine, but the machine handling queries made to the website could be completely different, but it is presented to you as if they are one machine.

- Embedded OS
	- Embedded OS's are made for a specific purpose, for example a washing machine's OS does not need to have access to the internet or have a graphical user interface. 
	- Instead, they are built to complete the simple task that they are for, using as little processing power as well, with maximum efficiency, using very little memory.

- Real Time OS
	-  In safety critical environments, e.g. aircraft autopilot, self drive cars or even missile systems, processes need to be guaranteed to be processed within a given time frame.
	- These often require a lot of capacity in memory and storage, as you cannot risk the OS being overloaded, and not being able to cope with the volume of tasks. As such, real time operating systems hardly ever run at full capacity.


# Virtual Machines, Bios, and Device Drives

## BIOS 

- BIOS stands for Basic Input Output System, it is responsible for loading operating systems when the PC is booted, as well as some basic diagnostics, such as the power-on-self test (POST).
- The BIOS keeps track of many of the important information about the hardware of the pc, such as fan speed, temperature etc.
- The bootstrap is used to load the OS kernel into memory, where at this point the OS can take over the rest and boot everything else
	- The initial start up instructions are stored in the ROM, and the BIOS settings are stored in flash memory, so it can be changed while also being retained.
