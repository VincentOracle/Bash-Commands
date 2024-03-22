## Bash Commands
In repository we have explored some Bash commands with examples

### Author: Were Vincent
### Date: 22 March 2024



### Practice 1
#### Screenshot 1


1.VAR1=”Hello World” creates a variable called VAR1 with the string value “Hello World”

2.echo $VAR1 prints the value of VAR1 which is the string value “Hello World”.

3.set | grep VAR1 searches for environment variables that contain the string "VAR1" in their names.

4.env | grep VAR1 is used to display the environment variables and then filter the output to only show lines containing the string "VAR1". It displays no output since VAR1 is not yet an environment variable

5.export VAR1 sets the environment variable VAR1 and makes it available to other processes and subprocesses

6.env | grep VAR1 is used to display the environment variables and then filter the output to only show lines containing the string "VAR1". Now it displays VAR1 and its value “Hello World”

7.PS1='C:${PWD////\\\\}>' sets the shell prompt (PS1) to display the drive letter "C:" followed by the current working directory, where forward slashes ("/") in the path are replaced with backslashes ("\"). The prompt will end with a ">".

8.cat ~/.bash_profile prints out the contents of the bash_profile file

9.cat ~/.bashrc prints out the contents of the bashrc file

### Practice 2
#### Screenshot 2


1.lpadmin -p km1 -E -v /dev/null -m raw adds a printer named "km1" without a physical connection (-v /dev/null) using a raw print queue (-m raw).

2.lpadmin -d km1  sets the default printer to "km1"

3.cupsaccept km1 is used to enable accepting print jobs for a printer named "km1" in the Common Unix Printing System (CUPS). This command allows the specified printer to start processing print jobs that are submitted to it.

4.cupsdisable km1 used to disable a printer named "km1" in the Common Unix Printing System (CUPS).

5.lpstat -t is used to display the status of the printing system and all of its printers in a detailed format. It provides information about the status of each printer, such as whether they are enabled, disabled, or idle, as well as any print jobs that are in the queue.

6.less /etc/cups/printers.confThe is used to view the contents of the `printers.conf` file, which is a configuration file for printers in the Common Unix Printing System (CUPS). The `less` command allows you to paginate through the file, making it easier to read large files.ings.

7.lp /etc/issue sends the contents of the `/etc/issue` file to the default printer for printing.

8.lpstat display status information about the current print jobs.

9.ls /var/spool/cups lists the contents of the CUPS (Common Unix Printing System) spool directory. In a CUPS system, this directory is where print jobs are temporarily stored before being sent to the printer for processing.



### Practice 3
#### Screenshot 3



1.cd classfiles changes the current working directory to the directory ‘classfiles’

2.tar -zcvf /sample.tar.gz Poems creates a compressed archive file named "sample.tar.gz" containing the file "Poems".

3.tar -ztvf /sample.tar.gz lists the contents of the compressed archive file named "sample.tar.gz" without extracting them.

4. mkdir test1 && cd test1creates a directory named test1 and changes directory to it.

5.tar -zxvf /sample.tar.gz extracts the contents of the compressed archive file named "sample.tar.gz" in the current working directory.

6.ls -R will list files and directories recursively.

7.Cd /classfiles changes the working directory to classfiles.

8.find Poems | cpio -vocBL -O /sample.cpio creates a CPIO archive named "sample.cpio" containing the contents of the "Poems" directory and its subdirectories.

9.cpio -Bitv -I /sample.cpio extracts the contents of the CPIO archive file "sample.cpio" and displays information about the extraction process.

10.mkdir test2 && cd test2 creates a new directory named "test2" in the current working directory and then changes the current working directory to "test2”.

11.cpio -vicdumB -I /sample.cpio extracts the contents of the CPIO archive file "sample.cpio" while displaying detailed information about the extraction process. #

12.dnf install dump is used to install the "dump" package using the DNF package manager.

13.dump -0uf /sda1.dump0 /dev/sda1 creates a level 0 backup of the "/dev/sda1" filesystem and writes the backup to a file named "/sda1.dump0."

14.dump -1uf /sda1.dump1 /dev/sda1 creates a level 1 dump of the filesystem on `/dev/sda1` and saves it to the file `/sda1.dump1`.

15.cat /etc/dumpdates displays the contents of the "/etc/dumpdates" file. This file typically contains a record of the last time the "dump" utility was used to back up file systems on the system, including information about the devices, dates, and levels of the dumps performed.

16.dd if=/dev/sda1 of=/sda1.dd creates a disk image file named "sda1.dd" by copying the contents of the "/dev/sda1" partition.

17.df -hT is used to display information about disk space usage in a human-readable and tabular format.

18.ls -l /sda1.dd lists detailed information about the file named "sda1.dd" in the root directory, including file permissions, ownership, size, and modification time.
