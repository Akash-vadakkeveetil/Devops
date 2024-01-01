<h1 align="center">Linux File System 📂</h1>
<hr>
### Linux File system VS Windows File system

The Linux file system is a hierarchical system, it is just like a tree structure a shown below

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

While in windows, there are multiple root folders. It was from older times when floppy disks were used each folder were assigned to separate disks, and they were named based on alphabets like :, B:  etc

The letters A: and B: were given to the removable disk and when hard drives were added the value C: is given to it. And it stayed the same to this day.

### Linux file system Overview 

So let's go ahead and cover the folders inside the root folder 

#### /Home 📂
Every user will their own space for files in the home directory. So in the root directory there will be a folder home which contains all the user's separate home folders. 

#### /bin 📂

Stands for binaries. Contains the most basic commands available in Linux , such as cp, cat etc. These all commands are in the binary files so that the system understands it. 

#### sbin 📂

