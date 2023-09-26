# Operating Systems

- The operating system is a platform for the software of a computer to be able to communicate with the hardware.
- For example, one feature that modern operating systems have is ***Multitasking***
	- Multitasking is where you can have more that one program running at the same time. 
	- What a single core multitasking system does, is allocate a small amount of time to each process, and switch between them at a speed that we don't notice the gaps in-between.

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