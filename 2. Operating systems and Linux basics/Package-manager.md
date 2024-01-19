
<h1 align="center">Package manager on Linux ➡️</h1>
<hr>


90% Applications are installed on Linux with the help of package managers and not like we install in the Windows systems .

So what is a software package ? - A software package is a bundled collection of programs, scripts, and related resources designed to perform specific tasks or functions on a computer system programs

Role of package manager - Each software have certain dependencies in it. So during installation, the files in the software package are basically assigned to different folders along the Linux file system. Package manager helps us find the dependencies and then store in different folders during installation and when uninstalling the software or application they are removed from the respective folders automatically.

On Ubuntu, we have a package manager called APT (advanced package tool)

#### 🍂 Some basic commands

`apt` - displays the commands and actions which can be performed using the APT
`sudo apt search <package name>` - to search for a package
`sudo apt install <package name>` - to install a package
`sudo apt remove <package name>` - to remove a package
`sudo apt update` - refreshes the package list on a Linux system,
`sudo apt upgrade` - installs the available updates for the installed packages.

APT-GET is another package manager on Linux, but we prefer apt more because it is more user-friendly than apt-get, and also it does not have the search option which is present in the apt

So where do these software packages get stored ?? They are stored in repositories over the internet. So before installing a package on Linux, we run `sudo apt update` to refresh and get the latest versions of the packages from the database.
The URL of the repositories which the package manager will use to find the package is in the file `sources.list`

### Other methods to install software except apt

- If an application is not possible to install through apt, then we can use the Ubuntu software application to install apps from. It is like an app store or play store.

### By using Snappy

 Another method for installing without the apt is by using another software manager called Snappy. The command for snappy is `snap`.

### Difference
| Snappy | Apt |
| ---- | ---- |
| Self-contained - dependencies                                  <br>contained in the package |   Dependencies are shared |
| Supports universal Linux packages<br>(package type .snap) | Only for specific Linux distributions<br>(package type .deb) |
| Automatic Updates | Manual Updates |
| Larger Installation Size | Smaller Installation Size |

That means when we download a package dependency will be downloaded and then if we install the same package, the dependency will be downloaded multiple times but in apt it will not happen because dependencies are shared. So apt does better management in it.


## By using Add repository 

If the software is not in the current available repository used by apt, we have to manually add a new repository and then install the package. If we add the repo, it will be automatically added to the sources.list file.
We can also create a PPA, that is personal private archive.

- **PPAs (Personal Package Archives):** Community-driven repositories enabling individuals to create private software distribution channels.
    
- **Developer Usage:** Often employed by developers for quicker software updates compared to official Ubuntu repositories.
    
- **Cautionary Notes:**
    
    - **Quality and Security:** No guaranteed standards for quality or security.
    - **Compatibility Risks:** Similar to other unofficial packages, PPAs can pose difficulties during system upgrades, particularly when moving to a new Ubuntu release.



 >The Debian Linux systems uses apt or apt-get, while the red hat distributions uses YUM