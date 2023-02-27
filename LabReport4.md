# Lab Report 4

## Step 4: Log in to ieng6
First, I opened my remote terminal then type the command ```ssh cs15lwi23ang@ieng.ucsd.edu``` which is my username ieng6. Since 
I have done the ssh-keygen step, signing in has been made easy, as it no longer requires the user to input their password. 
once I have type in my ieng6 ID, I pressed ```<enter>``` which prompted me that I have successfully logged in. 


<img width="519" alt="login" src="https://user-images.githubusercontent.com/122497280/221509949-86169881-0fb4-4afc-9bc5-34f9db329eb7.png">

---

## Step 5: Clone your fork of the repository from your Github account
For this step, I started by typing the command ```git clone``` followed the ssh key that I copied over from github, then pasted the 
ssh key after the ```git clone``` command I put in. After everything was typed in, I pressed ```<enter>``` to run the command, prompting me 
with a succesful clone. 


<img width="742" alt="image" src="https://user-images.githubusercontent.com/122497280/221512249-05155f25-6adb-40f4-9138-1835f8d21fd5.png">


---


## Step 6: Demonstrate that tests fail
First, in order to be able to show the test cases failing, you need to compile the ListExamples.java file. But in order to do that, you must first change its directory. The command to do so is ```cd``` then pressing ```<l>``` then pressing ```<tab>``` to autocomplete it 
as ```lab7/```. What pressing ```<tab>``` does is the terminal autocompleting the word so it saves the user a bit of 
typing and spelling errors. Now that we are in the target file's directory, we use the compile command ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java``` then press ```<enter>```. After we have compiled the file, we then run the exectute command: ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples``` then press ```<enter>```. This is what it should look like: 

<img width="654" alt="Screen Shot 2023-02-27 at 12 49 44 AM" src="https://user-images.githubusercontent.com/122497280/221516794-d4364655-9e10-4080-a161-e193b2807259.png">

---


## Step 7: Fixing the error 
To fix the error, we have to access the code through the terminal. To do this, use the command ```nano ListeExamples.java``` then press ```<enter>```. This should bring you to the nano screen where you see the ListExamples.java file. The error was changing the index incrimentation but instead of having 
it be ```index1```, it should be ```index2```. To be able to change this, you should be able to scroll down to the target line, then press ```<right>``` 12 
times, then press ```<backspace>``` then pressing ```<2>```, thus replacing the 1 with a 2. Now you need to save your changes and exit the terminal.
This can be done by pressing ```ctrl + o``` then pressing ```<enter>```. Then to exit, press ```ctrl + x```.

<img width="413" alt="image" src="https://user-images.githubusercontent.com/122497280/221519652-4e26011d-9887-4cc1-b743-2a3e4eb8bad1.png">


<img width="265" alt="image" src="https://user-images.githubusercontent.com/122497280/221519412-45169178-6d24-4698-a5fe-64dff2e70742.png">

---


## Step 8: Demonstrating that tests succeeded. 
Very similar to step 6, we use the compile and execute command, only that this time, we don't have to change our directory. So similar to before, we paste 
the compile command, ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java``` then press ```<enter>```. Now we execute to see if the code is working by pasting the execute command: ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExmaples``` then press ```<enter>```. Shown by the picture, we now pass the tests. 

<img width="654" alt="image" src="https://user-images.githubusercontent.com/122497280/221522535-ad468ca7-0eb2-46c4-a2bf-0eace8494483.png">

--- 

## Step 9: Push changes to Github
To push the changes to Github, use the command ```git add``` followed by the target file name which would ```ListExamples.java```. The whole 
command should look like ```git add ListExamples.java```, then press ```<enter>```. After that, we want to commit the file to github by using the
command ```git commit -m``` followed by a desired string which is to be put in quotes. The command I used was ```git commit -m "FileUpdate``` then 
I pressed ```<enter>```. You will prompted by the follwing which contains file status updates. 


<img width="504" alt="image" src="https://user-images.githubusercontent.com/122497280/221524721-80599002-9f26-40cf-b02e-a09cfa52b59f.png">

