## TASKS TO PERFORM :- 

### 1. Put master.txt on master branch, stage and commit
### 2.Create 3 branches: public1, public2 and private 
### 3.Put public1.txt on public 1 branch, stage and commit
### 4. Merge public 1 on master branch 
### 5. Merge public 2 on master branch 
### 6.Edit master.txt on private branch, stage and commit 
### 7.Now update branch public 1 and public 2 with new master code in private
### 8. Also update new master code on master
### 9.Finally update all the code on the private branch

### SOLUTION:-

  ![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/c5ea1cc4-e85d-4ff6-b9b9-35007a8c01a0)

### STEP1: -
First, on our Ubuntu server, we created a directory named "task1" using the command "mkdir task1". Then, we navigated into the "task1" directory. Inside it, we created a file named "master.txt" and initialized a Git repository by typing "git init". This means we're now using Git to track changes to our files. Next, we added "master.txt" to the Git repository, indicating that Git should keep track of changes to that file. After that, we committed our changes using "git commit -m", effectively creating a branch called "master". To confirm this, we used the command "git branch".

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/ea74122a-06eb-46ad-b47e-6cd266ddce52)

### STEP2: - 
After creating the initial "master" branch, we proceeded to create three additional branches: "public1", "public2", and "private", using the command "git branch". Then, we switched to the "public1" branch by checking it out using the command "git checkout public1". Inside this branch, we created a file named "public1.txt" using the command "touch public1.txt". Following that, we added "public1.txt" to the staging area for Git to track changes using the command "git add public1.txt". Finally, we committed the changes made to "public1.txt" using the command "git commit".

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/bacffd44-f22f-4302-803d-ec2d5b300c14)


### STEP3: -
After completing work on the "public1" branch, we switched back to the "master" branch by using the command "git checkout master". Then, we merged the changes from the "public1" branch into the "master" branch with the command "git merge public1". Subsequently, we repeated the process for the "public2" branch by merging it into the "master" branch using the command "git merge public2". However, when attempting to merge "public2" into "master", Git displayed the message "Already up to date", indicating that there were no differences between the "master" branch and the "public2" branch at that time. This means that the changes made in the "public2" branch had already been incorporated into the "master" branch through previous merges or commits.

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/5e4ae7f5-d648-4f97-9cfe-ae47f79d86eb)

### STEP4: - 
After switching to the "private" branch using the command "git checkout private", we proceeded to modify the "master.txt" file. We made these modifications using the text editor "nano". Upon saving the changes and exiting the editor, we checked the status of our Git repository using the command "git status", which revealed that "master.txt" had been modified. To stage the changes made to "master.txt" for committing, we used the command "git add master.txt". This command tells Git to track the changes made to "master.txt". Finally, we committed the modifications to "master.txt" to the "private" branch using the command "git commit". This action saves the changes to the Git history, making them a part of the "private" branch's version of "master.txt".

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/915d0c5e-ad59-4650-ae0c-45b3b7b704c1)

### STEP5: - 
After making modifications to the "master.txt" file in the "private" branch, we aimed to update the "public1" and "public2" branches with these changes. Firstly, we checked out the "public1" branch using the command "git checkout public1". Then, to integrate the changes from the "private" branch into the "public1" branch, we executed the merge operation with the command "git merge private". Subsequently, we repeated the same process for the "public2" branch. We checked out the "public2" branch using the command "git checkout public2", and then merged the changes from the "private" branch into the "public2" branch using the command "git merge private". By performing these steps, we successfully updated both the "public1" and "public2" branches with the modifications made in the "private" branch. This ensures that all branches now have the latest version of the "master.txt" file.

