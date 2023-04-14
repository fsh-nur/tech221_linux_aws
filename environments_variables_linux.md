# Environements in linux

## How to provision an environment in linux using bash script

1. Launch an instant

![1  Launch Instance](https://user-images.githubusercontent.com/129324316/232101833-d9a0be87-2d9b-4858-a57e-dac8b8f19ccc.png)


2. Name your instant and choose your AMI

![2  Input Name and AMI](https://user-images.githubusercontent.com/129324316/232101913-1d5be5b7-facf-418d-975e-4fb46c440218.png)

3. Input key pair and select existing security group

![3  Input key pair and select existing security group](https://user-images.githubusercontent.com/129324316/232102090-6649a367-80d8-44dc-83ab-7aeb40f3d8c3.png)

4. Click on advanced details

![4  Click on advanced details](https://user-images.githubusercontent.com/129324316/232102105-2bc50b3d-0cef-477a-88cc-e6b48816a8db.png)



5. Input bash script here in this format

![5  Input bash script here in this format](https://user-images.githubusercontent.com/129324316/232102124-e3bc2f6e-71fa-4ea3-9a8e-c976e385dda1.png)

```
#!/bin/bash 
sudo apt update -y 
sudo apt upgrade -y 
sudo apt install nginx -y 
sudo systemctl restart nginx 
sudo systemctl enable nginx
```
6. Connect your ssh client
![6  Connect your ssh client](https://user-images.githubusercontent.com/129324316/232102782-dd8dd0fe-615e-4d76-b769-1f976b398687.png)


7. Locate your IP address

![7  locating public ip](https://user-images.githubusercontent.com/129324316/232102926-357521b2-54fd-4e3b-ad46-c50980f926c1.png)

8. Input into the web to see if it works
![7  Input ip address](https://user-images.githubusercontent.com/129324316/232102810-e1179c6f-3980-4096-93e7-05583d037aaa.png)


## Finding environment variables/ variables in linux

`printenv` - prints all existing environment variables
`printenv PWD` - locating an environemnt variable with a specific name

![locationg environemtn variable](https://user-images.githubusercontent.com/129324316/232076097-15f135ef-2032-47e5-acff-bf8a88846f74.png)

`env` - another way of seeing environment variable


## Creating a variable in linux
1. Creating a variable and calling it :
 `MY_NAME=fatima`
 `echo $MY_NAME`
 
 ![CREATING A VARIABLE AND CALLING IT](https://user-images.githubusercontent.com/129324316/232075927-ad11708e-e8a6-44bc-9324-4c1c48762f4a.png)
 
## Creating an environmental variable
Creating an environemnt variable: `export LAST_NAME=sheikhnur`

![environemnt variable](https://user-images.githubusercontent.com/129324316/232076816-6d4dd050-1772-4151-a0c7-344ee8909f04.png)


**However once you leave the environment this variable it will be gone**
We can check if the environmental variable is still present by exiting and entering back into linux
`exit` and `enter` and then typing `printenv LAST_NAME` to locate the specific variable. It will not be present.
This is why it is important to create a **persistent** environmental variable.

## Creating a **persistent** environmental variable
1. Enter the command `ls -a` in order to see the hidden files within linux
2. `nano .bashrc` will take us to the bashrc document this is where we will enter our variable in order for it to remain persistent and present.
3. `export name = fatima` we will enter this command and input our chosen variable.
4. `CTRL + X` and `yes` to save the document
5. Now we can test to see if our variable is still present.
6. Input the command `source .bashrc`
7. Now we input `printenv name` in order to search for our variable within .bashrc
8. We locate the variable 


![persistent environment variable](https://user-images.githubusercontent.com/129324316/232078452-6ca0c278-f589-4b09-857c-a88c43f5a830.png)


