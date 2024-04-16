### Tasks to perform

1. Create a git flow workflow architecture on git 
2. Create all the required branches 
3. Starting from the feature branch, push the branch to the master, following the architecture 
4.Push a urgent.txt on master using hotfix

### solution:-

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/275be314-8934-4e4d-bbb8-5660d3770435)

## STEP1: - 
This is the diagram we have to follow this. we begin by creating the "master" branch and adding the "master.txt" file to it. Next, we create a branch named "develop" from the "master" branch. Inside the "develop" branch, we add the "develop.txt" file. Within the "develop" branch, we create another branch called "feature" where we add the "feature.txt" file. Once the work on the "feature" branch is complete, we merge its changes back into the "develop" branch. Then, we merge the changes from the "develop" branch back into the "master" branch. Finally, we create a new branch named "hotfix" from the "master" branch and add the "urgent.txt" file within this branch.


![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/488e2fd4-56a2-4c7f-b919-c5d720c44d1b)

## STEP2: -
To begin, we initialize a Git repository in our project directory using the "git init" command. Following this, we create the "master.txt" file. To add "master.txt" to the staging area for committing, we use the "git add master.txt" command. Then, we commit the changes to "master.txt" using the "git commit -m" command with an appropriate commit message. Next, we create a new branch called "develop" using the "git branch develop" command, and then switch to the "develop" branch using the "git checkout develop" command. Within the "develop" branch, we create a new file named "develop.txt" using the "touch develop.txt" command. We add "develop.txt" to the staging area with "git add develop.txt", and then co.mmit the changes to "develop.txt" using "git commit -m". Continuing, we create a new branch called "feature" using the "git branch feature" command, and switch to the "feature" branch using "git checkout feature". Inside the "feature" branch, we create a file named "feature.txt" and commit it similarly to the previous steps

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/b1bf2107-1e60-47d2-bf22-cc419209aec7)

## STEP3: 
After completing work in the "feature" branch, we switch back to the "develop" branch using the command "git checkout develop". Then, we merge the changes from the "feature" branch into the "develop" branch using the command "git merge feature". Following that, we switch to the "master" branch using the command "git checkout master". From the "master" branch, we merge the changes from the "develop" branch using the command "git merge develop". This process integrates the changes made in the "feature" branch into the "develop" branch and then merges the changes from the "develop" branch into the "master" branch, ensuring that the latest developments are incorporated into the main branch.

![image](https://github.com/satyamaatmdeep10/Git-Practice/assets/137147966/81cdf9a0-3732-4730-999b-5d8b0225be26)

## STEP4: 
Once we're on the "master" branch, we create a new branch called "hotfix" using the command "git branch hotfix". Inside the "hotfix" branch, we create a file named "urgent.txt" using any text editor or the "touch" command. We then add this file to the staging area using "git add urgent.txt", and subsequently commit it using "git commit -m 'Added urgent.txt for hotfix'". After committing the changes in the "hotfix" branch, we switch back to the "master" branch using the command "git checkout master". Once back on the "master" branch, we merge the changes from the "hotfix" branch into the "master" branch using the command "git merge hotfix". After merging, if we list the files using the "ls" command, we should see all the files including "urgent.txt" present in the "master" branch, confirming that the hotfix has been successfully applied.



