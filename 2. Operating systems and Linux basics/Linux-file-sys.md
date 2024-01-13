<h1 align="center">Linux 🐧and Linux File System 📂</h1>

<hr>

> 
### 🍂 Linux: An In-Depth Exploration and its Enduring Popularity

Linux, an open-source operating system (OS), stands as a robust force in the realm of computing, seamlessly running on a diverse array of devices, including servers, desktops, laptops, cloud environments, and mobile devices. Rooted in the Unix operating system, Linux has evolved over decades, originally serving as a platform for scientific and academic computing. Its popularity stems from various factors that contribute to its versatility and widespread adoption.

#### **Open Source Foundation**

At its core, Linux's strength lies in its open-source nature. This characteristic empowers users to access and modify its source code freely. This open philosophy fosters collaboration and innovation, enabling a vast community of developers and users to collectively enhance and refine the system continually.

#### **Security Prowess**

Noteworthy among Linux's attributes is its robust security infrastructure. The operating system benefits from a vigilant community that diligently identifies and addresses security vulnerabilities. The collaborative effort in addressing potential threats ensures a proactive stance against emerging challenges, making Linux a trusted choice for security-conscious users.

#### **Customizability Unleashed**

Linux stands out for its unparalleled customizability, allowing users to tailor the system to meet their specific requirements. From the kernel level to the user interface, Linux offers a high degree of flexibility, making it an ideal choice for users seeking a personalized computing experience. This adaptability extends to diverse use cases, from embedded systems to high-performance computing clusters.

#### **Community-driven Development**

The expansive community surrounding Linux plays a pivotal role in its ongoing success. Comprising developers, enthusiasts, and users worldwide, this community is characterized by its passion for the platform. Collaboration within this ecosystem results in rapid problem-solving, continuous improvement, and the development of a rich repository of resources, further solidifying Linux's standing as a reliable and constantly evolving OS.

#### **Versatile Deployment**

Linux's versatility is evident in its deployment across a wide spectrum of devices and environments. From the backbone of web servers to the efficiency of desktop computing, Linux adapts seamlessly to diverse scenarios. Its presence in cloud computing and mobile devices further underscores its adaptability, catering to the evolving needs of the digital landscape.

In conclusion, Linux's enduring popularity can be attributed to its open-source foundation, robust security, unmatched customizability, vibrant community, and adaptability to varied computing environments. As technology continues to advance, Linux remains a stalwart choice for those seeking a powerful, flexible, and community-driven operating system

  

### 🏗️ Key Architectural Components Shaping Linux 

  **Kernel:** At the core of Linux, the kernel manages hardware resources, ensuring seamless communication between software and hardware. It establishes a stable interface for smooth interaction.

**System Libraries:** These pre-written code repositories provide common functions, promoting efficiency and consistency across diverse applications on the Linux platform.

**User Space:** The realm of applications, from text editors to web browsers, offering users a diverse and rich computing experience.

**Shell:** A powerful command-line interface enabling users to execute commands, script automation, and navigate the OS with precision.

**System Utilities:** Compact programs designed for specific tasks, enhancing overall OS functionality, including file management, process oversight, and network administration.

**Daemons:** Operating in the background, daemons execute continuous tasks crucial for system functionality, such as managing network services and handling log data.

**Configuration Files:** Blueprints for tailoring Linux OS, allowing customization of network settings, system configurations, and security parameters.
  

![architecture](https://user-images.githubusercontent.com/37767537/225990738-9e505c6d-bad0-4820-a2b2-4ce84ef286c9.jpg)

  

### 🍂 Linux Distributions

  

Linux's distributions, also known as "distros," are different versions of the Linux operating system that are built And packaged with specific versions of the architectural components, the package management system used, the graphical user interface, and the tools and applications included in it.

  

Examples of Linux distros include Ubuntu, Fedora, Debian, CentOS, Mint, Red Hat Enterprise Linux (RHEL), etc.

  

### 🍂 Linux File Systems

  

The Linux file system is the way that the operating system organizes and stores files and directories on a computer's hard drive or other storage devices. It consists of a hierarchical structure where files and directories are arranged in a tree-like format starting from the root directory (represented by "/"). Each file and directory has a unique location within the file system hierarchy, and these locations can be referred to using a path, similar to how file paths work in other operating systems.

  

There are several types of file systems available for use on Linux, including below:

  

- Ext4: This is the most widely used file system on Linux, and it is known for its high performance, reliability, and scalability. It is a journaling file system, meaning that it keeps track of changes made to the file system in a log that helps to ensure that data is not lost in the event of a system failure.

  

- XFS: This is a high-performance file system that is optimized for large-scale data storage and is commonly used in enterprise and high-performance computing environments. It supports large file sizes and high-bandwidth I/O which makes it well-suited for use with high-speed storage devices such as solid-state drives.

  

- Btrfs: This is a newer file system that is designed to be flexible, scalable, and easy to manage. It offers advanced features such as snapshots which allow administrators to easily backup and restore data, and it also supports data and metadata checksums which help to prevent data corruption.

  

- NTFS: This is a file system commonly used in Microsoft Windows, and it is supported by most modern Linux distributions. It is designed to be compatible with a wide range of devices including hard drives and removable storage devices, and it supports advanced features such as compression and encryption.

  

- FAT32: This is an older file system that is commonly used in older Microsoft Windows systems and is also widely used for removable storage devices such as USB drives and has limitations such as a maximum file size of 4GB.

  
<h2> 🍂Linux File system VS Windows File system</h2>

The Linux file system is a hierarchical system as mentioned above, it is just like a tree structure a shown below

```markdown
root
	├── home
	│   ├── user1
	│   │   ├── Documents
	│   │   └── Pictures
	│   └── user2
	│       ├── Documents
	│       └── Music
	├── var
	│   ├── log
	│   └── www
	└── etc
	    ├── config
	    └── ssh

```

While in windows, there are multiple root folders. It was from older times when floppy disks were used each folder were assigned to separate disks, and they were named based on alphabets like :, B:  etc

The letters A: and B: were given to the removable disk and when hard drives were added the value C: is given to it. And it stayed the same to this day.

## 🍂 Linux file system Overview 

So let's go ahead and cover the folders inside the root folder 
>To visit your root folder on Ubuntu, Files ⇾ other locations ⇾ computer


```markdown
├── bin  -> usr/bin
├── boot
├── cdrom
├── dev
├── etc
├── home
├── lib           -> usr/lib
│   ├── lib32     -> usr/lib32
│   ├── lib64     -> usr/lib64
│   └── libx32    -> usr/libx32
├── lost+found
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin          -> usr/sbin
├── snap
├── srv
├── sys
├── tmp
├── usr
└── var

```

#### /Home 📂
Every user will their own space for files in the home directory. So in the root directory there will be a folder home which contains all the user's separate home folders. 

#### /bin 📂

Stands for binaries. Contains the most basic commands available in Linux , such as cp, cat etc. These all commands are in the binary files so that the system understands it. 

#### sbin 📂

System Binaries. Other type of commands which need superuser permission to execute. These are commands like 'Change password'

#### /lib 📂

Library folders, which hold libraries for the commands.

#### /usr 📂

Stands for user, these were the folder for the user before the home folder was introduced. So when we look into this folder there are many folders including the bin folder also. IT holds commands similar to the /bin folder. These are due to the historic reasons, back in the days when the Unix was developing due to storage limitations the directory was split into root binary folders and user binary folders. Now it doesn't make any sense.

The third party applications which we install will go to <code>/usr/local </code>folder. Local folder also contains many subfolders, so the different parts of the installing application will go to different place, like documentation will go to one folder, libraries will go to another etc.

#### /opt 📂

Stores third party applications which we installed as user. So what is the difference between these <code>opt</code> and <code>usr</code> folder ? 
So there are some applications which will not split its components and store it in different places like we said above, they store it in one single directory. In examples, most of the IDE which we use.

#### /boot 📂

contains files needed for booting the system including the Linux kernel and boot loader configuration files 

#### /etc. 📂

Et cetera, folder to store configuration settings and files.

#### /dev 📂

Stands for devices. The devices which we connected to our system will be here, like keyboard, mouse.

#### /var 📂

Contains files to which the system writes to during the course of its operation, like cache.

#### /tmp 📂

To temporarily store data when some process is being executed in the background.

#### /media 📂

Contains subdirectories, where removable media devices inserted into the computer are mounted, E.g. when you insert a CD. A directory will automatically be created, and you can access the contents of the CD inside the directory
### /mnt 📂

Historically, sysadmins mounted temporary file systems there.


## Hidden files 

Hidden files, also known as dot files in UNIX systems, are files that have filenames starting with a dot (.) character. They're primarily used to prevent accidental deletion of important data and are automatically generated by programs or the operating system. These files are hidden from view by default in file browsers or directory listings to maintain a cleaner and less cluttered display. In UNIX systems, appending a dot before a folder or file name effectively hides it from normal view, keeping the directory structure cleaner and preventing accidental modifications to critical system files.



>NB:The subdirectories might differ across various Linux distributions, but the fundamental structure remains consistent. Exploring each subdirectory individually is highly advised to gain a better understanding of its contents.