## Lab Report 1

## Task 1: Streamlining ssh Configuration

- Show your .ssh/config file, and how you edited it (with VScode, another program, etc)


<img width="570" alt="Screen Shot 2022-04-28 at 7 47 29 PM" src="https://user-images.githubusercontent.com/65454241/167285188-903df1cd-b4cb-418c-a3e4-1bc09645f6a0.png">


<img width="827" alt="Screen Shot 2022-05-07 at 11 47 54 PM" src="https://user-images.githubusercontent.com/65454241/167285210-b9dea650-ac3d-4dc1-be9b-b59efa463820.png">


- Show the ssh command logging you into your account using just the alias you chose.

<img width="559" alt="Screen Shot 2022-05-07 at 11 50 40 PM" src="https://user-images.githubusercontent.com/65454241/167285286-1ddc7abb-9294-41c3-843d-5923f3dc9d48.png">


- Show an scp command copying a file to your account using just the alias you chose.

<img width="543" alt="Screen Shot 2022-05-07 at 11 56 15 PM" src="https://user-images.githubusercontent.com/65454241/167285470-e26194a9-2daf-4479-bd47-341f4c5ccc17.png">



In the above tasks I added a series of steps to our config file and logged into our server using the simple command of `ssh ieng6`. Following this I made a file using touch and copy pasted it using the `scp` command into our remote server. 


## Task 2: Setup Github Access from ieng6

- Show where the public key you made is stored on Github and in your user account (screenshot).

<img width="500" alt="Screen Shot 2022-05-08 at 12 01 59 AM" src="https://user-images.githubusercontent.com/65454241/167285605-8e6a6efc-f3bd-40df-aad4-0b54074fe3da.png">


<img width="562" alt="Screen Shot 2022-05-08 at 6 46 39 PM" src="https://user-images.githubusercontent.com/65454241/167327082-b2227880-1c66-4e0a-b0e7-1a3b2d4821dd.png">




- Show where the private key you made is stored on your user account (but not its contents) as a screenshot.


<img width="396" alt="Screen Shot 2022-05-08 at 6 49 24 PM" src="https://user-images.githubusercontent.com/65454241/167327294-21a0ff19-46f2-4098-95aa-a12b4c72be8f.png">



- Show running git commands to commit and push a change to Github while logged into your ieng6 account.


<img width="767" alt="Screen Shot 2022-05-08 at 4 54 49 PM" src="https://user-images.githubusercontent.com/65454241/167321063-4ef01ec7-b8f0-4a23-af04-c6d911cff3d6.png">

- Show a link for the resulting commit.
[link](https://github.com/KSB2003/markdown-parser/commit/23c91d7a97288c0e2e9da4f1469966f3d448cdf2)



I created the key and stored it in github. I navigated to the file with the key in the system and performed a `cat` command in order to see the contents of the key. Then I ran the neccessary git commands and pushed a change to github from our ieng6 account. 



## Task 3: Copy whole directories with scp -r

- Show copying your whole markdown-parse directory to your ieng6 account.


<img width="259" alt="Screen Shot 2022-05-08 at 5 10 52 PM" src="https://user-images.githubusercontent.com/65454241/167321759-eff8eb36-c77d-405a-a7ca-515b14178938.png">


- Show logging into your ieng6 account after doing this and compiling and running the tests for your repository.


<img width="1600" alt="Screen Shot 2022-05-08 at 5 20 55 PM" src="https://user-images.githubusercontent.com/65454241/167321936-d7a38ef1-7672-4032-86e6-292b09b18f7e.png">

- Show (like in the last step of the first lab) combining scp, ;, and ssh to copy the whole directory and run the tests in one line.

<img width="571" alt="Screen Shot 2022-05-08 at 6 09 16 PM" src="https://user-images.githubusercontent.com/65454241/167324604-53c6b32a-b39d-454d-b9ba-88dc9b630579.png">


<img width="343" alt="Screen Shot 2022-05-08 at 6 12 51 PM" src="https://user-images.githubusercontent.com/65454241/167324683-23cf054e-2545-4815-9a38-2ecaac8f77f9.png">

I copied the entire directory using `scp -r` and then I logged into my account and ran the markdown parser. I then combined all of the steps using semicolons and ran it all at once. 

