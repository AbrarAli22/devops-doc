ubuntu commands

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