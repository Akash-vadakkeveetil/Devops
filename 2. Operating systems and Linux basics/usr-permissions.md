<h1 align="center">Linux accounts and user permissions 🧾</h1>
<hr>

## 🍂Types of accounts
#### Superuser Account

The superuser, often referred to as the root user, has unrestricted permissions on a Linux system. This account is used for administrative tasks. To perform administrative tasks, one can either log in directly as the root user or execute commands with elevated privileges using the `sudo` command.

#### User Account

A user account is created for regular usage and login. For example, a user named "tom" might have a home directory located at `/home/tom`.

#### Service Account

Service accounts are created for specific services like Apache or MySQL on Linux server distributions. Each service gets its dedicated user account. For instance, a "mysql" user might be created to run the MySQL application. It's a best practice for security not to run services with the root user to minimize potential vulnerabilities.

## 🍂 Best Practices for Security

- **Avoid Root User for Services:** Do not run services with the root user to limit the potential impact of security vulnerabilities.
- **Dedicated Service Accounts:** Create individual user accounts for each service to isolate and control permissions effectively.
- **Limited Permissions:** Grant only the necessary permissions to each user or service account to reduce the risk of unauthorized access or misuse.
- **Use sudo:** When administrative tasks are required, prefer using the `sudo` command to execute commands with elevated privileges instead of logging in as the root user.


	In windows, a centrally managed system is present in case of user accounts, but on Linux it is absent. That is the reason why most of the companies and universities users windows as their OS for employees and students. So on Linux it is different from one computer to another, that is if there are accounts, their info is stored in that specific computer itself.


### Group and Permissions

When we have to provide certain permissions for different people, we basically make a group and add them to that group so that we don't have to assign permissions individually. When that person is removed from the group, permissions are lost.


Example:

`Akash: x: 1000: Akash,, : / home/ akash: /bin/bash`

GENERAL FORMAT :

`USERNAME : PASSWORD : UID : GID : GECOS : HOMEDIR : SHELL`

**Password** - x means, that encrypted password is stored in /etc/shadow file

**User ID (UID)** -  Each user has a unique ID. UID 0 is reserved for root

**Group ID (GID)** - The primary group ID (stored in /etc/group file)

**User ID Info** - Comment Field for extra information about user

**Home directory** - Absolute path of user's home directory

**Default Shell** - Absolute path of a shell

adduser <username> = create new user
Automatically chooses policy-conformant UID and GID values
Automatically creates a home directory
with skeletal configuration

passwd <username> =
Change password of a user

su - <username> =
Login as username
su = short for substitute or switch user

groupadd <groupname> =
Create new group
By default, system assigns the next available GID
from the range of group IDs specified in the login.defs file

we can find groups in /etc/group
Different User & Group Commands
adduser

addgroup
deluser
delgroup

Interactive
More User Friendly
Easier to use!
Like it chooses conformant UID and GUID values for you
Creates a home directory with skeletal config automatically
Or asks for input in interactive mode

(when using manyuaaly)

useradd
groupadd

userdel
groupdel

You need to provide the infos yourself
Low-level utilities

(use these type command in scripts when u are executing it ina automated way)

usermod [OPTIONS] <username> =
Modify a user account

`sudo usermod -g DeVops Akash` - The user named Akash will be inside the DevOps group now or we can also say that this user's primary group will be DevOps

`sudo usermod -G admin,other gorups Akash` - to add Aksh in multiple secondary gorups

`sudo usermod -G admin Aksh ` - overrides every other preexisting group and adds the user to the freshly crealted group

`sudo usermod -aG newGroup Akash - to append one more group

'groups' - displays which all groups are the logged user present in

`groups Akash` - to see which all groups user is in without logging in as that user.

useradd [OPTIONS] <username> =
Create a new user
The low-level command compared to "adduser"
-G create user with multiple secondary groups
-d custom home directory
and other options for shell, etc.


