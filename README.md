# OperatingSystem
## Introduction:
• Operating system is intermediatary between system hardware and applications installed.
• OS is the base for the applications or programs it holds.
• Various types of OS: Batch type, Time based OS, Single processor OD, Multi Processor OS
• Operating system:
1. Interaction between hardware and software
2. Holds responsibility of allocating resources to users and for each and every program
3. It does the management of processes, security and more
4. Every program first needs to be loaded into main.memory and then display it on the screen, user changes are later saved into secondary storage and this complete job is done by OS
5. Without OS every task we need to write many lines of code, which is tedious for normal user to operate a system
# OS provides:
1. Provides convenience to the user to use
2. Efficient use of space and memory
• CPU is small unit of the mother board
• Motherboard contains alot like disk controller, video adapter, usb controller which are controlled by small chip CPU
• A general purpose computer system has one or more cpu's, with several device controllers, connected via common bus that gives access to shared-memory
• CPU and Device controllers can work concurrently in memory cycles
• Memory controller synchronizes every task to perform concurrently
[  ] Boostrap program is the intial program that runs( that is loaded onto ram 1st ) when you turn on the system, code is stored in ROM.
Its functionality is to start the OS program, os is stored in harddisk which more size than RAM,so bootstrap is a program knows where OS is installed and this bootstrap program starts the OS.

Later the kernel of the operating system after the intiation of bootstrap program, it will load the OS onto RAM.
[  ] Interrupt, usually hardware interrupts the CPU, through system bus, then CPU must stop the process its doing, & responds to the interrupt.
[  ] System Call, usually when the software interrupts the CPU then it is called (system call or monitor call)
[  ] Interrupt Service routine,  means that CPU responds to the interrupt by immediately stoping its current task and transfers it to a fixed location.
And then the service routine contains the starting address of the task paused.
Later the after the completion of task, they will resume the interrupted service routine. And completes that task too.
• Registers (smallest unit of memory,fast access of data) that can be accessed  --》 Cache (little slower than registers) --》 Main memory (RAM, Limited space, volatile in memory)--》 Electronic tapes--》Optical disks --》 Magnetic tapes .
( Top to bottom  access time increases, and cost per bit decreases, size of items are also increases )
• Only at the time of execution code is loaded into primary memory, from secondary memory (bookself and table is an example of memory types)
• Usually big Main memory or RAM fastly they gets loaded than low RAM
• Storage is one of the many types of IO devices, basically large part OS code is only to cordinate IO devices, and coordinating them makes the system efficient and gives better performance.
• Each device controller is incharge of specific type of devices, 
each device controller maintains
1. Local Buffer storage 
2. set of special purpose registers
• Every OS has specific type of device drivers for each device,which provide interface between device controĺler and device( if device controler is unable to access the device its respective device driver is installed and used to communicate via device controller)
 • Here in the IO operations device co troller sends an interrupt when the data is loaded from device to registers. And its comoletion triggers cpu to hold on and allocate memory to the loaded data.
• This will cause cpu being interrupted everytime (for every bit of data that is uploaded into memory) and its not that efficient way, so we added Direct Memory Access control(DAM) to directly allocate memory (into buffer storage in memory) without interrupting CPU everytime.
• By tgis Direct access memory, we can have only 1 interrupt after sending entire block of data not just bit-by-bit
# Computer system Architecture:
• Computer systems are divided based on general purpose registers:
1. Single processor systems
2. Multi processor systems
3. Clustered systems
## Note:
 CPU  is capable of executing the instruction set also including instructions from user processes.
• Not just the CPU ,we have other general purposes processors designed to work for a device specific tasks
[  ] Advantages of mutli processor systems vs single processor systems:
1. High throughput - due to parallel task performance
2. Economical is better - 3 individuals systems needed with 3 individual resources whereas for multiprocessor systems single resource is shared to use its maximum efficiency via single storage.
3. Reliable - even if one processor fails rest are there to manage at SPOF

## Multi processesing systems are of 2types:
 Clustered systems:
 Similar to systems tasks done are also classified as:
1. Mulit programming:
 2. Multi tasking or Time sharing system
  [  ] A process is a program that is loaded into the memory and when its starts executing is known as PROCESS
# OS services:
 1. User interface 
2. Program execution
3. IO operations
4. Files management and access privelages management
5. Communication between processes inside CPU (necessary between processes to be in sync with status of other process and to go and execute after one by one completion in same or diff computers)
6. Error detection (like papers not available in printer in this error case prpgram shouldnt terminate completly there should be error handling mechanism done by os)
7. Resource allocation to each of the process
8. Accounting of each every user activity and also resources
9. Protection & security ( no other user can manipulate data, and in process level other processes shoulf not directly interfere with running process directly this is done by os to protect the current process)
A chain is as strong as its weakest link
