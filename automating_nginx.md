# Automating the process of installing nginx

1. Create a shell script
![image](https://user-images.githubusercontent.com/129324316/232018086-caa3992b-208f-447d-aefe-0be882296780.png)
`nano provision.sh` to create a shell script called provision
2. Enter this script entailing what each step does
![bashscripting](https://user-images.githubusercontent.com/129324316/232018538-663679b9-9bdd-4d65-a16d-2bcbe97b3998.png)
3. `CTRL + X` then `yes` to save
4. Change permissions so you can execute it:
`sudo chmod +x provision.sh
5. Run the script:
`sudo ./provision.sh`
6. We then check to the status and making sure everything is running with the below command.
`sudo systemctl status nginx`
7. Copy your public IPv4 addres and pate it in a new window in your internet browser to open the page
8. You will see this image once opened:
![image](https://user-images.githubusercontent.com/129324316/232021021-dec8015c-e2b7-44ba-bb88-e4924ca4be76.png)


