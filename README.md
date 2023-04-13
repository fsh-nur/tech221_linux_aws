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
-Setting permissions so only you (owner) can read/write/execute:
`chmod 700 tech221.txt`

# Security groups in AWS

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




