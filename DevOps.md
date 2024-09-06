ubuntu commands
  
  system users commands
  
  
  
  
  
  
  
  
  
  commands that use admin prevliage
  1. Add a new user  sudo adduser username
  2. add a new user sudo useradd username
  3. delete or modified user sudo deluser username 
  4. sudo usermod options username
  5. sudo passwd username to change userpassword
  6. unlock useraccount sudo usermod -U username
  
  
  testing script
  
  how script worksh


1) Ls command
ls command is used for list the data inside the directory ls is also used with some flags to inhanse the functionality here are some of them
ls -l : this means list shown in long format like detail
ls -s : this means list to shown by file size
ls -ha : Show long format ﬁles and directories including hidden ﬁles
ls -lh :list long format ﬁles and directories with readable size

2) Cd Command :

cd means change directory 
cd then the directory name and user move from that directory to other directory in a maner way
cd .. means back to previous directory or up directory.

3) Cat command
cat command is used to creat a new file or open that specific file if exist
cat means concatenate.
cat is used todisplay the contant of the file on terminal.
syntax cat > filename ,cat > filename,file2,file .....
we can creat multiple files at a time using this .
cat * .file type is used to open same file type in that specific directory
cat * is used to display all the files in that current directory 
cat filename > file2 this > operator shows that user is coping the data of file one in file2 it means it vanish the data in the target file if it have any data and copy the frist file data only
cat >> it means to append the data in the file .
cat file1 file 2 merge_file3 this will seprate the both files data and merge the data of both file in a new file
cat -n file name shows the line numbers 

4) Tac command 
it is reverse of cat command
it also use concate methode 

5) head command 
   head command use to show default the top 10 means the first 10 entreys or lines
   head command also used with parameter  
   head command with -n flag then pass specific integer number to see that records from the top of file  command : head -n <number> foo.txt
   
6)  tail command
it is reverse of head command and useful to see log file it shows the latest 10 records of the file 
we can also see more then 10 records using this command with -n flag then pas 

7) pwd command
it prints the current working directory
this can also di=one by echo $pwd variable

8) touch command
touch command is used to modifies the timestamp of that file or if he file does not exist 
it is used for modification of files

9) cal command 
calendar is display with this command 
	we can also see specific calendar with the command cal 
	Usage: cal [general options] [-jy] [[month] year]
       cal [general options] [-j] [-m month] [year]
       ncal -C [general options] [-jy] [[month] year]
       ncal -C [general options] [-j] [-m month] [year]
       ncal [general options] [-bhJjpwySM] [-H yyyy-mm-dd] [-s country_code] [-W number of days] [[month] year]
       ncal [general options] [-Jeo] [year]
General options: [-31] [-A months] [-B months] [-d yyyy-mm]
10) bc command 
it is used to perform mathematical operation in terminal
11) df command
it means disk free this command is used to check the storage or space
we can use different formats to see data like mb gib or bytes etc
12) help command 
it is used to see command that are available 
this also willl use with specific command that the command have functionality etc
13) uname
this command is used to see system informations

14) The mkdir command
is used to creat directory 

15) gzip
it is used to compress and decompress the data or files
gzip file name or directory.
gzip -d file name or directory
gzip -r directory_name use to compress directory or folder
gzip -dr directory_name use to decompress directory or folder

16) What is
this is used to see what a unknown command can do eg whatis ls
17) who
who command is used to display loggedin users and current run level of system and the last system boot
1. Print out all details of currently logged-in users
who -a
2. Print out the list of all dead processes
who -d -H

who [options] [filename]
Additional Flags and their Functionalities
Short Flag
Description
-rprints all the current runlevel
-dprint all the dead processes
-q print all the login names and total number of logged on
users
-hprint the heading of the columns displayed
-b print the time of last system boot

18) Free
this is used to show or see memory information
19) top/htop command
it is pre build command It is used for displaying information about the system and its top CPU-consuming processes as well as RAM usage. it is like as ps command
from top get back command is press q for exit;
we can filer process using awk command with specific filters to get specific processes
htop is a tool to monitor the process and manage with more attractive colors and functionality
Comparison between top and htop:
20) echo
echo used to print the line and save the test in a file or append lines in files

21) finger
it is external program used to see user info or a particular user
22)groups
 it shows the or manage the user with the same prevlage 
 23) cp
 cp means copy command it used to copy a file or multiple files or folder/directory 
 1. To copy the contents of the source ﬁle to the destination ﬁle.
cp sourceFile destFile
If the destination ﬁle doesn't exist then the ﬁle is created and the
content is copied to it. If it exists then the ﬁle is overwritten.
2. To copy a ﬁle to another directory specify the absolute or the
relative path to the destination directory.
cp sourceFile /folderName/destFile
3. To copy a directory, including all its ﬁles and subdirectories
cp -R folderName1 folderName2
If the destination directory already exists, the source directory itself and
its content are copied inside the destination directory.
4. To copy only the ﬁles and subdirectories but not the source
directory
cp -RT folderName1 folderName2
24) mv command
used to move files or directory frome one to another it is also used to rename a file or folder
1. To rename a ﬁle called old_name.txt:
mv old_name.txt new_name.txt
2. To move a ﬁle called essay.txt from the current directory to a
directory called assignments and rename it essay1.txt:
mv essay.txt assignments/essay1.txt
3. To move a ﬁle called essay.txt from the current directory to a
4. directory called assignments without renaming it
mv essay.txt assignments

25) ps command
The ps command is used to identify programs and processes that are
running on the system and the resources they are using. Its frequently
pipelined with other commands like grep to search for a
program/process or less so that the user can analyze the output one
page at a time.
26) kill command
 kill command in Linux (located in /bin/kill), is a built-in command
which is used to terminate processes manually. The kill command
sends a signal to a process which terminates the process. If the user
doesn’t specify any signal which is to be sent along with kill command
then default TERM signal is sent that terminates the process.

27) killall command
killall sends a signal to all processes running any of the speciﬁed
commands. If no signal name is speciﬁed, SIGTERM is sent. In general,
killall command kills all processes by knowing the name of the
process.
Signals can be speciﬁed either by name (e.g. -HUP or -SIGHUP) or by
number (e.g. -1) or by option -s.
If the command name is not a regular expression (option -r) and
contains a slash (/), processes executing that particular ﬁle will be
selected for killing, independent of their name.
killall returns a zero return code if at least one process has been
killed for each listed command, or no commands were listed and at
least one process matched the -u and -Z search criteria. killall
returns non-zero otherwise.
A killall process never kills itself (but may kill other killall
processes).
Examples:
1. Kill all processes matching the name conky with SIGTERM:
killall conky
# OR
killall -SIGTERM conky
# OR
kilall -15 conky
I was able to kill Wine ( which are Windows exe ﬁles running on Linux )
28) env command
The env command in Linux/Unix is used to either print a list of the
current environment variables or to run a program in a custom
environment without changing the current one.
1. Print out the set of current environment variables
env
2. Run a command with an empty environment
env -i command_name
3. Remove variable from the environment
env -u variable_name
4. End each output with NULL
env -0
29) printenv
The printenv prints the values of the speciﬁed environment
VARIABLE(s). If no VARIABLE is speciﬁed, print name and value pairs for
them all.
Examples:
1. Display the values of all environment variables.
printenv
2. Display the location of the current user's home directory.
printenv HOME
3. To use the --null command line option as the terminating
character between output entries.
printenv --null SHELL HOME
NOTE: By default, the printenv command uses newline as the
terminating character between output entries.
30) nano command
it is an editor like vi and vim it also creat file if the file not exist
its a pre-build editor
31) rm command
rm which stands for "remove" is a command used to remove (delete)
speciﬁc ﬁles. It can also be used to remove directories by using the
appropriate ﬂag.
32) ifconfig command
ifconfig is used to conﬁgure the kernel-resident network interfaces. It
is used at boot time to set up interfaces as necessary. After that, it is
usually only needed when debugging or when system tuning is needed.
If no arguments are given, ifconfig displays the status of the currently
active interfaces. If a single interface argument is given, it displays the
status of the given interface only; if a single -a argument is given, it
displays the status of all interfaces, even those that are down.
Otherwise, it conﬁgures an interface.
33) ip command
The ip command is present in the net-tools which is used for
performing several network administration tasks. IP stands for Internet
Protocol. This command is used to show or manipulate routing, devices,
and tunnels. It can perform tasks like conﬁguring and modifying the
default and static routing, setting up tunnel over IP, listing IP addresses
and property information, modifying the status of the interface,
assigning, deleting and setting up IP addresses and routes.
34) clear command
it is used to clear the terminal screen
35) su command
it is used to switch the user eg su then the user name if no name is given is proceed to root user
36) wget command
The wget command is used for downloading ﬁles from the Internet. It
supports downloading ﬁles using HTTP, HTTPS and FTP protocols. It
allows you to download several ﬁles at once, download in the
background, resume downloads, limit the bandwidth, mirror a website,
	and much more.
	
37) curl command
In linux, curl is a tool to transfer data from or to a server, using one of
the supported protocols(DICT, FILE ,FTP, FTPS, GOPHER, HTTP, HTTPS,
IMAP, IMAPS, LDAP, LDAPS, POP3, POP3S, RTMP, RTSP, SCP, SFTP, SMB,
SMBS, SMTP, SMTPS, TELNET and TFTP).
38) yes command
it is used to print endless string in terminal
39) last command
This command shows you a list of all the users that have logged in and
out since the creation of the var/log/wtmp ﬁle. There are also some
parameters you can add which will show you for example when a
certain user has logged in and how long he was logged in for.
40)locate command
it is used to search specific file or folder location which matches
41)sudo command
is used to intract with root user 
The sudo ("substitute user do" or "super user do") command allows a
user with proper permissions to execute a command as another user,
such as the superuser.
This is the equivalent of "run as administrator" option in Windows. The
sudo command allows you to elevate your current user account to have
root privileges. Also, the root privilege in sudo is only valid for a
temporary amount of time. Once that time expires, you have to enter
your password again to regain root privilege.

42)apt command
it is used to install applications in os/and remove that pakage/upgrade
apt (Advantage package system) command is used for interacting with
dpkg (packaging system used by debian). There is already the dpkg
command to manage .deb packages. But apt is a more user-friendly
and eﬃcient way.
In simple terms apt is a command used for installing, deleting and
performing other operations on debian based Linux.
You will be using the apt command mostly with sudo privileges.
Installing packages:
install followed by package_name is used with apt to install a new
package.
Syntax:
sudo apt install package_name
43) zip command
The zip command is used to compress ﬁles and reduce their size. It
outputs an archive containing one or more compressed ﬁles or
directories.
44) shutdown command
The shutdown command lets you bring your system down in a secure
way. When shutdown is executed the system will notify all logged-in
users and disallow further logins. You have the option to shut down your
system immediately or after a speciﬁc time.
Only users with root (or sudo) privileges can use the shutdown
command.
45) dir command
The dir command lists the contents of a directory(the current directory
by default). It diﬀers from ls command in the format of listing the
content. By default, the dir command lists the ﬁles and folders in
columns, sorted vertically and special characters are represented by
backslash escape sequences.
46)reboot command
The reboot command is used to restart a linux system. However, it
requires elevated permission using the sudo command. Necessity to
use this command usually arises after signiﬁcant system or network
updates have been made to the system.
47)sort command
the sort command is used to sort a ﬁle, arranging the records in a
particular order. By default, the sort command sorts a ﬁle assuming the
contents are ASCII. Using options in the sort command can also be used
to sort numerically.
48) paste comand
The paste command writes lines of two or more ﬁles, sequentially and
separated by TABs, to the standard output
49)exit command
it is used to close or terminate the active shell session 
ctrl + D is also a shortcut to exit the process and terminal.
50) diff/sdiff command
This command is used to display the diﬀerences in the ﬁles by
comparing the ﬁles line by line.
51) tar command
it is used to compress and un-compres the files and folders
The tar command stands for tape archive, is used to create Archive
and extract the Archive ﬁles. This command provides archiving
functionality in Linux. We can use tar command to create compressed
or uncompressed Archive ﬁles and also maintain and modify them.
52) gunzip command
The gunzip command is an antonym command of gzip command. In
other words, it decompresses ﬁles deﬂated by the gzip command.
gunzip takes a list of ﬁles on its command line and replaces each ﬁle
whose name ends with .gz, -gz, .z, -z, or _z (ignoring case) and which
begins with the correct magic number with an uncompressed ﬁle
without the original extension. gunzip also recognizes the special
extensions .tgz and .taz as shorthands for .tar.gz and .tar.Z
respectively.
53) hostnamectl
The hostnamectl command provides a proper API used to control Linux
system hostname and change its related settings. The command also
helps to change the hostname without actually locating and editing the
/etc/hostname ﬁle on a given system.

54) scp command
secure copy command it allows to copy file from different location in encrypted format so at trafic no one can see the sensitve data
55)sleep command
The sleep command is used to create a dummy job. A dummy job helps
in delaying the execution. It takes time in seconds by default but a
small suﬃx(s, m, h, d) can be added at the end to convert it into any
other format. This command pauses the execution for an amount of
time which is deﬁned by NUMBER.
Note: If you will deﬁne more than one NUMBER with sleep command
then this command will delay for the sum of the values.
56)split command
The split command in Linux is used to split a ﬁle into smaller ﬁles.
57)useradd command
The useradd command is used to add or update user accounts to the
system.
To add a new user with the useradd command the syntax would be the
following:
useradd NewUser
To add a new user with the useradd command and give a home
directory path for this new user the syntax would be the following:
useradd -d /home/NewUser NewUser
To add a new user with the useradd command and give it a speciﬁc id
the syntax would be the following:
useradd -u 1234 NewUser

58)userdel command 
The userdel command is used to delete a user account and related
ﬁles
Examples:
To delete a user with the userdel command the syntax would be the
following:
userdel userName
To force the removal of a user account even if the user is still logged in,
using the userdel command the syntax would be the following:
userdel -f userName
To delete a user along with the ﬁles in the user’s home directory using
the userdel command.

59)usermod command
The usermod command lets you change the properties of a user in Linux
through the command line. After creating a user we sometimes have to
change their attributes, like their password or login directory etc. So in
order to do that we use the usermod command.

60)ionice command
The ionice command is used to set or get process I/O scheduling class
and priority.
If no arguments are given , ionice will query the current I/O scheduling
class and priority for that process.
61)ping command
The ping (Packet Internet Groper) command is a network utility used to
check network connectivity between a host and a server or another
host. It sends ICMP (Internet Control Message Protocol) echo requests to
a speciﬁed IP address or URL and measures the time it takes to receive
a response. This time delay is referred to as "latency." Ping is a
fundamental tool for network troubleshooting and monitoring.
62)rsync command
The rsync command is probably one of the most used commands out
there. It is used to securely copy ﬁles from one server to another over
SSH.
Compared to the scp command, which does a similar thing, rsync
makes the transfer a lot faster, and in case of an interruption, you could
restore/resume the transfer process.
In this tutorial, I will show you how to use the rsync command and copy
ﬁles from one server to another and also share a few useful tips!
Before you get started, you would need to have 2 Linux servers. I will
be using DigitalOcean for the demo and deploy 2 Ubuntu servers.
You can use my referral link to get a free $100 credit that you could use
to deploy your virtual machines and test the guide yourself on a few
DigitalOcean servers:
**Transfer Files from local server to remote**
This is one of the most common causes. Essentially this is how you
would copy the ﬁles from the server that you are currently on (the
source server) to remote/destination server.
What you need to do is SSH to the server that is holding your ﬁles, cd to
the directory that you would like to transfer over:
cd /var/www/html
And then run:
rsync -avz user@your-remote-server.com:/home/user/dir/
The above command would copy all the ﬁles and directories from the
current folder on your server to your remote server.
Rundown of the command:
-a: is used to specify that you want recursion and want to preserve
the ﬁle permissions and etc.
-v: is verbose mode, it increases the amount of information you
are given during the transfer.
-z: this option, rsync compresses the ﬁle data as it is sent to the
destination machine, which reduces the amount of data being
transmitted -- something that is useful over a slow connection.
I recommend having a look at the following website which explains the
commands and the arguments very nicely:
**Transfer Files remote server to local**
In some cases you might want to transfer ﬁles from your remote server
to your local server, in this case, you would need to use the following
syntax:
rsync -avz your-user@your-remote-server.com:/home/user/dir/
/home/user/local-dir/
Again, in case that you have a non-standard SSH port, you can use the
following command:
rsync -avz -e 'ssh -p 2510' your-user@your-remote-
server.com:/home/user/dir/ /home/user/local-dir/

Transfer only missing files
If you would like to transfer only the missing ﬁles you could use the --
ignore-existing ﬂag.
This is very useful for ﬁnal sync in order to ensure that there are no
missing ﬁles after a website or a server migration.
Basically the commands would be the same apart from the appended --
ignore-existing ﬂag:
rsync -avz --ignore-existing   user@your-remote-
server.com:/home/user/dir/

63)ssh command
The ssh command in Linux stands for "Secure Shell". It is a protocol
used to securely connect to a remote server/system. ssh is more secure
in the sense that it transfers the data in encrypted form between the
host and the client. ssh runs at TCP/IP port 22.

64)chmod command
it is used to change the add and remove the  



**Bash scripting**
we can creat a bach file using multiple command like using cat ,nano,vim,touch but at the end of file is saved with the extention of .sh this means a bash file
and we can make it executable file using +x chmod we can also give or set the preority using chmod of the file

