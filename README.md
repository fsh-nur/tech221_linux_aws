# Linux Commands

- Creating a folder
`mkdir tech221`
- Creating a text file
`touch tech221.txt`
- Editing a text file
`nano tech221.txt`
- Saving a text file 
`ctr+X` then `Y`
- Copying a file from one place to another command, then the file you want to copy then the location
`cp tech221.txt tech221`
- Rmoving a file
`rm tech221.txt`
- Moving file state file first then location 
`mv tech221.txt tech221`
- Setting permissions so only you (owner) can read/write/execute:
`chmod 700 tech221.txt`
- Exit Linux terminal
`exit`
- Lists the details of all the files inside the folder.
`ll -a`
- Sudo grants admin permission.
`sudo <command>`
- Opens "task manager".
`top`
- Opens the .txt file with nano editor.
`nano <name>.txt`
- To know whether a process is running 
`ps aux | grep bash` processes runnning in the system using bash
- To kill process
`kill PID`
- Apt is a package manager for linux which keeps information on hand to install webservers such as nginx:
`sudo apt install nginx`
- Restart nginx
`sudo systemctl restart nginx`
- In order to update
`sudo apt update`
- Upgrade system and automate "continue"
`sudo apt upgrade -y`
- How to access the root
` sudo su`
- How to exit the root
`exit`



## Locating something from a file

Using HEAD

![head](https://user-images.githubusercontent.com/129324316/231771200-534084ec-3aa9-450c-a6c7-8cbd41ed0636.png)

As you can see, after running `head -1` the first line from the text file is shown


![image](https://user-images.githubusercontent.com/129324316/231772034-5fd897c1-c0bd-4905-bf80-f20f4d022099.png)
![nltech221](https://user-images.githubusercontent.com/129324316/231772066-99935934-b835-4d43-bf1e-52fd47c224e5.png)

Locating a file from the bottom
`tail -1`
