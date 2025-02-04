# 2.2 Cloning a GitHub Repository Using Visual Studio Code

## **Objective**:
- Understand how to clone a repository using Visual Studio Code.
- Gain familiarity with the Visual Studio Code interface and workflow.
- Prepare the cloned repository for development.

## **Prerequisites**:
1. Open **Visual Studio Code** on your machine. You can download it from [Visual Studio Code website](https://code.visualstudio.com/) .
2. Ensure you have a **GitHub account** and have the necessary access to the repository you want to clone.
3. Internet access for authentication and repository cloning.

## **Task 1: Cloning the Repository**

### Steps to Follow
1. Open **Visual Studio Code** on your machine. 
2. Click on **Clone Git Repository** view to clone the repository and paste the clone repo url from your GitHub account and press enter.
   
 ![image](https://github.com/user-attachments/assets/bfa57893-f7eb-4cee-ac6b-04949aa074be)


 ![image](https://github.com/user-attachments/assets/39cb61f6-8a06-4086-bbf5-618dd5e0cd47)


3. When prompted to sign in to GitHub, choose your GitHub account credentials or access Token. [Steps to create token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic) 

  ![image](https://github.com/user-attachments/assets/4f7e3e7e-1647-465e-86d3-721dbd22f26d)


### Task-2: Verifying the Clone and Create Developer Branch

1. Once the cloning process is complete, you will see the repository listed in Visual Studo Code.

  ![image](https://github.com/user-attachments/assets/a5026114-d0fc-4502-9498-0f88adeca1d3)


2. Navigate to the chosen directory on your local machine to verify the files have been successfully cloned.

   ![image](https://github.com/user-attachments/assets/fcb93a92-bc78-45b7-8a1f-34da6e66f2b9)

3. Go to the **Branch** section in Visual Studo Code and  Click **create new branch**.

  ![image](https://github.com/user-attachments/assets/1f2b38d5-476f-4635-8a29-01739addf4f2)
 
   
4. Enter the branch name `feature` and Press enter.

   ![image](https://github.com/user-attachments/assets/ccc3407e-6b13-4996-a136-96a191b2d5d7)

   
5. The new branch will be checked out automatically.

   ![image](https://github.com/user-attachments/assets/ff3eb0f9-b87f-4216-a79f-2aa1f1df22b1)


### Task-3 Modify Files Locally and Publish Changes to GitHub

1. Open the `Tailspin.SpaceGame.Web\Views\Home\Index.cshtml` file and make required changes.

2. Save your changes and Commit Changes Locally
   
3. you will see the modified changes listed, 

    ![image](https://github.com/user-attachments/assets/dcdee19e-cb39-4793-8fb1-9047fd0f4c96)

4. Enter a commit message with your issue no. for tracebility and click on **Commit**.

   ![image](https://github.com/user-attachments/assets/f137ecea-0a20-4c2d-ac39-bb9a4c7bef41)


   ![image](https://github.com/user-attachments/assets/02fe0664-6c2d-4228-ba48-3f5d8bc904b3)



5. Click the **Publish Branch** button, Your branch will be published to the remote repository successfully.
   
   ![image](https://github.com/user-attachments/assets/fc2fe359-e0ce-4ef1-8fc9-9c0db120ab73)

   ![image](https://github.com/user-attachments/assets/064f5d75-509f-4212-a8e8-603b730e8304)


### Outcome

At the end of the lab, participants should:
- Successfully clone a repository using Visual Studio Code.
- Be ready to start working on the cloned project locally.
- Create a feature branch, modify files, and commit changes locally.
- Publish their branch to the remote repository.
