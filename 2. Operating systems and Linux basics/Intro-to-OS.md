#### What is an operating system ??
Consider your computer as a hub with various hardware devices—such as printers, keyboards, and monitors—each having its own unique language or way of functioning. However, if you were to transfer data from one device to an application, it wouldn't be practical to write specific code in each application for accessing and interacting with each hardware component.

This is where the Operating System (OS) comes in. Acting as an intermediary, the OS bridges the gap between these applications and the hardware. It essentially serves as a mediator that understands the intricacies of different hardware languages. When applications need to interact with hardware, they communicate with the OS, which then manages the complexities of interfacing with the hardware. This allows the applications to focus on their specific tasks without having to worry about the technical details of how to communicate with individual devices. It also acts as a translator between hardware and system.
![os interaction diagram](IMAGES/os.png)

### Tasks of an operating system
- **Process management**  - processes are basically tasks which are currently being performed in the system, for example opening chrome, creating new file etc.
- **Memory management** - allocating working memory, because every application needs memory to work. The working memory is called RAM, which stands for rapid access memory. Since RAM is only limited so if new process comes and no RAM then OS does memory swapping and gives the new process (P2) the memory to execute and stores the previous executing process (P1) to the storage

![memory swap](IMAGES/memory_swapping.png)
- **Storage and File Management** - Also called the secondary memory and used to store data for a long time or permanently. The files are stored in a hierarchy structure. 
- **Management of IO devices** 
- **Security and networking** - OS will manage users and permissions. Each user can log in separately and each of the users have their own space. And in networking, OS assigns ports and IP addresses.