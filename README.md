# git_assignment_HeroVired

# Q.1: You are part of a development team working on a Python application called "CalculatorPlus." The application provides basic arithmetic operations, such as addition, subtraction, multiplication, and division. Your task is to implement a new feature that adds support for calculating the square root of a number.
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











# Q2.For a project that deals with large binary files, integrate Git LFS (Large File Storage) to handle these files efficiently. Demonstrate how to add, commit, and push binary files to the repository, ensuring they are tracked by Git LFS correctly. Clone the repository on another machine to verify that the binary files are downloaded correctly.

-----------------------
Step 1 : We need to install git lfs

#sudo apt update

#sudo apt install git-lfs

-----------------------
Step 2: We need to initilize the lfs into the github repository

#git lfs install

![image](https://github.com/user-attachments/assets/9f2f5d67-ee59-49b5-ba8b-9c736b72c91f)
![image](https://github.com/user-attachments/assets/c3afeda1-7510-4fca-abd9-e886d9603abb)

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




