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
sudo ./provision.sh
