# git_assignment_HeroVired
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


