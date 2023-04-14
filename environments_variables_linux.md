# Environements in linux

## How to provision an environment in linux using bash script

1. Naming the environment

![1  nameing](https://user-images.githubusercontent.com/129324316/232074574-91c5e967-47c2-4687-8318-d0dc840f228a.png)

2. Inputting the bash script used in order to install nginx within the "user_data! in "Adavanced Options" when scrolling down

![4  bash in user_data automation](https://user-images.githubusercontent.com/129324316/232074781-0792a45f-c01a-4167-ace7-4e333f00dd11.png)

3. Connect via ssh


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


