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




# Security groups in AWS and How to Create an Environment in AWS

## Creating an environment:
1. Click Launch an Instance
![image](https://user-images.githubusercontent.com/129324316/231810356-99a99c14-1b94-4dff-95ed-302d2314ef97.png)
2. If you do not have a template click launch instance in the drop down
![image](https://user-images.githubusercontent.com/129324316/231810651-50398fb3-025b-48ff-9aad-784732988edc.png)
3. Now you can configure your environment:
- Enter the name of your server
- Choose your AMI and choose your architecture
![image](https://user-images.githubusercontent.com/129324316/231811409-6f8d977a-a307-41ec-9017-d772248334a4.png)
4. Choose your instance type, instance type that you specify determines the hardware of the host computer used for your instance. 
![image](https://user-images.githubusercontent.com/129324316/231811574-d13468b9-42ab-4da8-af5b-d87f6666d6c1.png)
5. Choose your respective key-pair logins
![image](https://user-images.githubusercontent.com/129324316/231812515-33a82181-fb42-4f3a-95a6-dbdaa1940551.png)
6. Choose your network settings. Choose Create security group and make sure you choose allow ssh traffic from 
![image](https://user-images.githubusercontent.com/129324316/231813466-73155dc7-4a6c-44fe-957f-a494b12f1f7e.png)
7. Launch an instance 
![image](https://user-images.githubusercontent.com/129324316/231813981-f70d04ce-679f-4fad-b1d1-ec4d021f808b.png)



## How to create/edit/delete a security group:
1. Select your instance 
2. Click on the Security Tab shown
3. Click on the link to edit your security group

![image](https://user-images.githubusercontent.com/129324316/231761074-047626a7-6387-4a47-9373-da75cf2fa942.png)

4. Click on Action Tab
5. Select "Edit Inbound Rules"
![image](https://user-images.githubusercontent.com/129324316/231761615-a914fd63-9d52-41f4-a683-ee3adb752eb0.png)

6. Select Add Rule when you get to this page:
![image](https://user-images.githubusercontent.com/129324316/231761917-88b5a360-b083-42b0-8597-d763d359c329.png)

7. Select SSH as "Type"
![image](https://user-images.githubusercontent.com/129324316/231762254-c215f227-c31e-43a7-a093-d71e47d98fc5.png)

8. Select "My IP" as Custom
9. Click on Save Rules
![image](https://user-images.githubusercontent.com/129324316/231762564-13ff8a7a-7aef-4546-b9fd-35e9481edd98.png)

10. This message should pop up
![image](https://user-images.githubusercontent.com/129324316/231762705-9baa8506-a5eb-4a1b-92b9-2d1608b19cfc.png)

11. If you would like to delete the security group, click the delete button:
![image](https://user-images.githubusercontent.com/129324316/231763313-0103b453-ebe2-4db2-a5d5-7bc3e3600a1d.png)


## Connecting to Instance

1. Select your instance then click connect
![image](https://user-images.githubusercontent.com/129324316/231764332-a96e1c61-49c8-4c7d-9ff9-9ba2799e86d1.png)

2. Select the SSH Client Tab
![image](https://user-images.githubusercontent.com/129324316/231764633-7d3f0c88-9f93-4155-87a7-514bd029be9a.png)

3. Follow the instructions shown by opening up GitBash and directing to the ssh folder, where tech221.pem resides and running the command:
![image](https://user-images.githubusercontent.com/129324316/231765243-26cd48ac-22f3-40fe-ae0f-14bb3b03a1e3.png)

4. Run the command shown here in GitBash:
![image](https://user-images.githubusercontent.com/129324316/231765845-f8498645-8786-46df-b256-5fa5fc6702c8.png)

5. Once you run the command it will ask you these questions, type yes, this will take you to the linux terminal.

![image](https://user-images.githubusercontent.com/129324316/231766219-68a17763-e441-4b05-afd2-c436b09bf3f8.png)

![image](https://user-images.githubusercontent.com/129324316/231766520-61b0b9fc-03ea-48d2-8dde-c871afbb1393.png)


## Locating something from a file

Using HEAD

![head](https://user-images.githubusercontent.com/129324316/231771200-534084ec-3aa9-450c-a6c7-8cbd41ed0636.png)

As you can see, after running `head -1` the first line from the text file is shown


![image](https://user-images.githubusercontent.com/129324316/231772034-5fd897c1-c0bd-4905-bf80-f20f4d022099.png)
![nltech221](https://user-images.githubusercontent.com/129324316/231772066-99935934-b835-4d43-bf1e-52fd47c224e5.png)

Locating a file from the bottom
`tail -1`
