## Lab Report 1

**Part 1: Installing visual studio code**

Step 1: The first thing that must be done is dowloading visual studio code from the official website. You can use this [link](https://code.visualstudio.com/download) and download the appropriate version of visual studio code depending on the number of bits and the operating system that you are using.

Step 2: After installing you can access the zip file from your downloads and open it. This will look as follows (on MacOS):

<img width="290" alt="Screen Shot 2022-04-06 at 10 24 37 PM" src="https://user-images.githubusercontent.com/65454241/162126937-20b53f88-58ea-40e6-8baa-39cd69e07bac.png">

Step 3: Click on the zip file and take the following steps in order to be able to use visual studio and get it on your applications.


**Part 2: Remotely connecting**


Step 1: In order to remotely coonect to the server you must first be able to change your password for your UCSD account, you can do this via this [link](https://sdacs.ucsd.edu/~icc/index.php). It will look as follows:
<img width="869" alt="Screen Shot 2022-04-06 at 10 45 56 PM" src="https://user-images.githubusercontent.com/65454241/162128846-4452dc50-5626-470f-be9a-33d16e291c2a.png">


Step 2: Once you have done this you should be able to see your unique user code. It would be "cs15l22" followed by three letters that are unique to your account.

Step 3: Open up a terminal and type the following command in order to establish remote control. Also note that the hostname would follow the user and it would be '@ieng6.ucsd.edu'. Refer to the command below.

`$ ssh user@hostname`.

Step 4: After this you will be prompted to enter the password. The password will not actually show. This is expected and you should not worry as the password is hidden for security reasons. If you have correctly entered the password you should be able to enter. After you have logged in, it will look as follows:

<img width="400" alt="Screen Shot 2022-04-06 at 11 15 39 PM" src="https://user-images.githubusercontent.com/65454241/162132654-f1837158-e6a7-413c-9878-994c33aee266.png">


**Part 3: Trying some commands**


After you have connected there are a variety of commands that you could try on the remote server. 

`cd` - is a command that can help you navigate between the directories in the remote server.


`ls` - it is a command that lists all of the files in the current working directory in the remote server. 



You can create files with the following command:
`cat /home/linux/ieng6/cs15lsp22/public/hello.txt`

If you wish to logout of the remote server in your terminal you must run the following commands:
 - Ctrl-D
 - `exit`

The following is a picture of me attempting to access the remote server of one of my peers:


<img width="750" alt="Screen Shot 2022-04-07 at 12 07 28 AM" src="https://user-images.githubusercontent.com/65454241/162140391-43968014-2c38-4341-90ff-9b725280af53.png">




**Part 4: Moving files over SSH with scp**


Step 1: Create a random file on vs code. Make sure that the code actually compiles and save the file. Test the code by using `javac` and `java` on your computer. 

Step 2: Run the following command from the directory that contains the java file that you just created, find the command below (make sure you modify the user to your unique three letters):

`scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/`

Step 3: Login again with the ssh key onto ieng6 and use the `ls` command to list files. You shoud be able to see the file in the home directory on the remote server. You can even run the file using the `javac` and `java` commands on your computer. This works because java is already installed on the remote server. 


Step 3: Login again with the ssh key onto ieng6 and use the `ls` command to list files. You shoud be able to see the file in the home directory on the remote server. You can even run the file using the `javac` and `java` commands on your computer. This works because java is already installed on the remote server. The file will look as follows when it is run on the remote server:

<img width="700" alt="Screen Shot 2022-04-06 at 11 33 15 PM" src="https://user-images.githubusercontent.com/65454241/162135551-de3b9ccc-3ca9-4ecd-b1fb-de7ed01c77bc.png">


**Part 5: Setting up SSH keys**


Step 1: When you are on the client (your own computer not the remote server) type in the following command:

`ssh-keygen`

Step 2: You will receive a prompt telling you to enter a passphrase. Make sure you enter nothing and simply hit the enter button. It will ask for a confirmation again, click the enter button again. It will say that your identification has been saved and will display the randomart image. 

After you have logged in, it will look as follows:




<img width="700" alt="Screen Shot 2022-04-06 at 11 56 02 PM" src="https://user-images.githubusercontent.com/65454241/162138539-7953d067-801a-41d7-b690-d131d923c38b.png">




**Part 6: Optimizing Remote Running**


There are multiple ways in which you can optimize your remote running?:
 - You can directly type the following command while on your own system and see all of the files in the home directory of the remote server:


   `ssh cs15lsp22zz@ieng6.ucsd.edu "ls"`
   
   
 - You can also use semicolons in order to run multiple lines on the same command. For example:


   `cp WhereAmI.java OtherMain.java; javac OtherMain.java;
java WhereAmI`


This will look as follows:


<img width="850" alt="Screen Shot 2022-04-07 at 12 03 28 AM" src="https://user-images.githubusercontent.com/65454241/162139732-c1b744d5-a3c6-4b3e-963d-a739dd44407c.png">





