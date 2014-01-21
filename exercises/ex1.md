# Exercise 1

###1. Interrupts, I/O
* What is an interrupt? How can the system detect it?
* What may cause interrupt/exception? In what situations? What happens in the system then?
* What is the most common I/O technique used in the modern computers? How does it work?

###2. Program execution
* Sta12 Problem 1.2: The register level program execution of Figure 1.4 (lect01, slide 19) is described in the text using six steps. Expand this register level program execution to show the use of the MAR and MBR.
* Sta12 Problem 1.3: Consider a hypothetical 32-bit microprocessor having 32-bit instructions composed of two fields. The first byte contains the opcode and the remainder an immediate operand or an operand address.
  * What is ther maximum directly addressable memory capacity (in bytes)?
  * Discuss the impact on the system speed (in terms of number of memory ops) if the microprocessor has
    * a 32-bit local address bus and a 16-bit local data bus, or
    * a 16-bit local address bus and a 16-bit local data bus.
  * How many bits are needed for the program counter and th einstruction register?

###3. User mode vs kernel mode
* What is the difference between kernel and user mode? Explain why having two distinct modes aids in designing an operating system.
* Which of the following instructions should be allowed to execute only in kernel mode? (a) disable all interrupts, (b) read the time-of-day clock, (c) set the time-of-day clock, (d) change the memory map?

###4. OS overview
* What is the difference between OS and OS kernel?
* What is the relationship between multithreading, multicore, and SMP?
* Explain the difference between a monolithic kernel and a microkernel.
* Sta12 Problem 2.2: An I/O-bound problem is one that, if run alone, would spend more time waiting for I/O than using a processor. A processor-bound program is opposite. Suppose a short term scheduling algorithm favors those programs that have used little processor time in the recent past. Explain why this algorithm favors I/O-bound programs and yet does not permanently deny processor time from processor-bound programs.

###5. Cache
* In a CPU, cache access time is 500 ns and main memory access time is 2 µs. If a block is found, on average, 90% of the time in cache, what is the average access time?
* Continuing the preceeding a part, but varying the average cache hit ratio, make table with 80%, 85%, 90%, 95% and 99% averages. What can you deduce from the numbers?
* Sta12 Problem 1.13: A computer has a cache, main memory, and a disk used for virtual memory. If a referenced word is in cache, 20 ns are required to access it. If it is in main memory, but not in * cache, 60 nc are needed to load it into the cache (including the original time to check the cache), and then the reference is started again. If the word is not in main memory, 12 ms are required to fetch it from the disk, followed by 60 ns to copy it to cahce, and then reference is started again. The cache hit ratio is 0.9 and the main memory hit ration is 0.6. What is the average time in ns required to access a referenced word in this system?

###6. Virtualization
* How does virtual memory relate to physical memory? When would you want to use it? When not?
* What is a Virtual Machine Monitor (VMM)? Give a practical example relating to Linux fork() system command when host operating system is Windows.
* What is a Process Virtual Machine (Fig. 2.14a, Le01 slide 55)? When would you want to use it?
* What is a System Virtual Machine (Fig. 2.14b, Le01 slide 56)? When would you want to use it?
* If you would want to run concurrently many applications with different operating systems, would you use a process or a system VM?
