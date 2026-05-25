# Linux_and_Server_assessment_Sandhya
Linux and Server assessment Assignments
#Assignment 1

# 1. Create the directory /home/ec2-user/webapp/ with three subdirectories inside it: scripts/, logs/, and config/ using a single mkdir -p command.

<img width="1071" height="202" alt="image" src="https://github.com/user-attachments/assets/bcbbda81-84c2-4cf9-9ffc-59835e6500e1" />

#2. Use cat > to create config/app.conf with two lines of content: APP_NAME=WebApp and PORT=8080. Save using Ctrl+D.

<img width="677" height="87" alt="image" src="https://github.com/user-attachments/assets/142f78b6-d462-43af-bb61-663c494352d3" />

#3.Use touch to create an empty file at logs/app.log. Confirm it is 0 bytes using ls -l.

<img width="758" height="96" alt="image" src="https://github.com/user-attachments/assets/f430d79b-b32f-4aee-bca0-a2dd58ee7782" />

#4.Set permissions: chmod 755 scripts/ and chmod 644 config/app.conf. Explain in your own words what 755 and 644 mean for owner, group, and others.

<img width="747" height="165" alt="image" src="https://github.com/user-attachments/assets/80d38b00-8f4c-4e3f-a4d2-90a3efd9faca" />

=====================================
Meaning of permissions:

Note:
value of :
read is = 4
write is = 2
execute is = 1
=======================================
Therefore, permissions given to the above files means:
1)  755 = rwxr-xr-x

Owner (7 = rwx) → can read, write, execute
Group (5 = r-x) → can read and execute, cannot write
Others (5 = r-x) → can read and execute, cannot write
=================================

2) 644 = rw-r--r--

Owner (6 = rw-) → can read and write
Group (4 = r--) → can read only
Others (4 = r--) → can read only
==================================

#5. Recursively change ownership of the entire webapp/ directory to root:root using chown -R. Then run ls -lR /home/ec2-user/webapp/ and share the output to confirm every file and folder shows root root as owner.

<img width="825" height="421" alt="image" src="https://github.com/user-attachments/assets/ff5791c9-cce0-4162-8c46-75b18921d4fb" />

=================================================================================================================================== 

#Assignment 2

#1. Use read -p to prompt the user to enter their name and store it in a variable called username.

#2. Use cat with the absolute path to display the contents of config/app.conf to the screen.

#3. Append a log entry to logs/app.log using echo >> in this exact format: Login: $username Date: $(date). Then display the full log file contents.


<img width="1092" height="623" alt="image" src="https://github.com/user-attachments/assets/b334be90-2ef4-48cc-afcd-bc53bba427f9" />

<img width="1082" height="632" alt="image" src="https://github.com/user-attachments/assets/01553899-f0cc-4409-b857-a0d0547fba1e" />


<img width="890" height="92" alt="image" src="https://github.com/user-attachments/assets/d158a7e5-4442-4419-b72a-96cd22bf6189" />


#4. Give the script execute permission with chmod +x and run it at least 3 times using different names (e.g., Chirag, Priya, Ravi) so the log file has multiple entries for Question 3.


<img width="796" height="457" alt="image" src="https://github.com/user-attachments/assets/888ae8ab-607c-4ebd-820a-b4c2f71c9fee" />

<img width="688" height="100" alt="image" src="https://github.com/user-attachments/assets/f6af4c31-5070-4747-bf0e-75f0bc2330d3" />

================================================================================================================================== 

# Assignment 3
#Question 3: User Management and File Permission Control

#Objective: Create 4 Linux users. Two of them must have write access to the log_user.sh script created in Question 2, and the other two must have read-only access. Use Linux groups and chmod to control this.

1. Create the writers group
    sudo groupadd writers

   <img width="767" height="433" alt="image" src="https://github.com/user-attachments/assets/2297adb6-f353-433c-9035-8dae16cdf1f0" />

2. Create 4 users with home directories

3. 







