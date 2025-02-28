# git_assignment_HeroVired

Q.1: You are part of a development team working on a Python application called "CalculatorPlus." The application provides basic arithmetic operations, such as addition, subtraction, multiplication, and division. Your task is to implement a new feature that adds support for calculating the square root of a number.
-----------------------
Step 1: Create github repository name **git_assignment_HeroVired**
![image](https://github.com/user-attachments/assets/f2271b71-1699-41f1-9251-97000ac41c92)

-----------------------
Step 2: Create dev branch and add code into the branch.

#git checkout -b dev

#git branch 

#git add Calculator.py

#git commit -m "Added the initial code"

#git push origin dev

![image](https://github.com/user-attachments/assets/fe6fc932-eefa-45a0-9ef2-1f5694a939a2)
![image](https://github.com/user-attachments/assets/ae49cd1e-0d64-47e2-900e-583b4d991bb2)
![image](https://github.com/user-attachments/assets/be121bc1-3f99-46bb-9548-1b9fd215b0e9)



-----------------------
Step 3: Merge dev branch to main branch and create tag Version 1.

#git checkout main

#git merge dev

#git tag "Version1"

#git push origin dev

![image](https://github.com/user-attachments/assets/a86890f2-b5d7-4d15-b7ca-5e5a373efada)
![image](https://github.com/user-attachments/assets/0eef2f70-e6d3-401e-80b2-23c8f531eee9)

-----------------------
Step 4: Create branch 'feature/sqrt' and merge the code with help of classmates

#git checkout -b feature/sqrt
![image](https://github.com/user-attachments/assets/005329bd-f919-4a2b-acf8-4fe24bf7ad98)

-----------------------
Step 5: Add the divide by 0 code.
![image](https://github.com/user-attachments/assets/b524b96b-dbd6-46ef-8e9c-b063acd831ca)



Q2.For a project that deals with large binary files, integrate Git LFS (Large File Storage) to handle these files efficiently. Demonstrate how to add, commit, and push binary files to the repository, ensuring they are tracked by Git LFS correctly. Clone the repository on another machine to verify that the binary files are downloaded correctly.

-----------------------
Step 1 : We need to install git lfs

#sudo apt update

#sudo apt install git-lfs

-----------------------
Step 2: We need to initilize the lfs into the github repository

#git lfs install

![image](https://github.com/user-attachments/assets/9f2f5d67-ee59-49b5-ba8b-9c736b72c91f)

-----------------------
Step 3: We need to Create binary file

#dd if=/dev/zero of=./binary_file bs=1024 count=204800
![image](https://github.com/user-attachments/assets/603a128e-91d2-4904-a0c7-c0b54b75b8e0)

-----------------------
Step 4: We need to track the Binary file and it will create .gitattributes

#git lfs track binary_file

![image](https://github.com/user-attachments/assets/00a4f569-6c7c-4dee-a108-06d710c0f7fd)


-----------------------
Step 5: Commit and Push the .gitattributes and large file

#git add .gitattributes binary_file

#git commit -m "Adding .gitattributes and binary file"

#git push origin lfs
![image](https://github.com/user-attachments/assets/f48fa864-0023-42ab-a4b6-0db00fc7d86d)

-----------------------
Step 6: Clone the repo in different system and check the both size

#git clone git@github.com:ssptr007/git_assignment_HeroVired.git

#cd git_assignment_HeroVired/

#git checkout lfs

#ls -lrt

![image](https://github.com/user-attachments/assets/3c4bab3a-eb3f-45d1-87b0-92d1687532a5)

![image](https://github.com/user-attachments/assets/040f4e22-6ad8-4c17-9339-1475ff4dd302)

![image](https://github.com/user-attachments/assets/eab1da66-70a5-4c95-a17a-e7bd76cbdf74)


Q.3: In this same GitHub repository, create a new branch **geometry-calculator**, we'll work on a simple Python program that calculates the area of a circle and the area of a rectangle. We'll use Git stash to switch between working on multiple features (calculating circle area and calculating rectangle area) without committing incomplete changes.

-----------------------
Step 1: Create a branch **geometry-calculator** and add the file and stash it.

#git checkout -b geometry-calculator

#git add geometrycalculator.py

#git stash

![image](https://github.com/user-attachments/assets/ad3cd286-d18b-4800-93d6-d1873aea66ef)

-----------------------
Step 2: Create branch **feature/circle-area** and add the circle related code and stash it.

#git checkout -b feature/circle-area

#git add geometrycalculator.py

#git stash

![image](https://github.com/user-attachments/assets/6dd542be-6299-475c-9b4b-4715b0a9d095)

-----------------------
Step 3: Create branch **feature/rectangle-area** and add the circle related code.

#git checkout -b feature/circle-area

#git add geometrycalculator.py

#git stash

![image](https://github.com/user-attachments/assets/dc1c1c45-0545-45ba-949b-1b34862cf1a3)

-----------------------
Step 4: Switch back to **feature/circle-area** branch and continue working on the circle area feature

#git checkout feature/circle-area

#git stash list

#git stash apply stash@{1}

#git add geometrycalculator.py

#git commit -m "Added the Circle feature"

#git push origin feature/circle-area

![image](https://github.com/user-attachments/assets/f0198808-3ec3-4129-b305-ccd10ac0056b)

-----------------------
Step 5: Switch back to **feature/rectangle-area** branch and continue working on the circle area feature

#git checkout feature/rectangle-area

#git stash list

#git stash apply stash@{1}

#git add geometrycalculator.py

#git commit -m "Added the Rectangle feature"

#git push origin feature/rectangle-area

![image](https://github.com/user-attachments/assets/541d3848-126b-4aa3-b263-c8e7d41374a1)

-----------------------
Step 6: Share the pull request from feature/circle-area and feature/rectangle-area dev. We need to resolve the conflict and run the python script
![image](https://github.com/user-attachments/assets/65c1c9c2-7944-4dcd-9ef7-3ea4577420e0)

As the functionality is working fine. We can merge this into main branch
![image](https://github.com/user-attachments/assets/9bbd3721-332b-4dc0-abba-110c7a18cdc6)
![image](https://github.com/user-attachments/assets/d068a7fe-8926-4115-9ac0-7c07166adcc5)











