# Create a Repository

## Objective
Learn how to create a new repository in GitHub and how to add a user as a collaborator to a GitHub repository and assign appropriate permissions. This exercise helps you understand the process of initializing repositories from pre-existing templates, the process of managing repository access and permissions to facilitate collaboration on projects.

## Prerequisites
- You must have a **GitHub account**. If you don't have, see "[Creating an account on GitHub.](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)"
- Basic knowledge of GitHub repositories.
- The GitHub username or email address of the user you want to invite.

## Task-1: Create a Repository

### Steps to Follow
1. Navigate to https://github.com/ and Sign in.
2. After sign in upper right side click on **+** to create a new repository

![image](https://github.com/user-attachments/assets/76046ec6-9b22-45eb-a82d-94d958a854ce)

3. In Create a new repository page, in the "Repository name" box, type `<repo-name>`.

4. In the "Description" box, type a short description. For example, type "This repository is for practising the GitHub Flow."

5. Select whether your repository will be Public or Private.

6. Select Add a README file and Click Create repository.

![image](https://github.com/user-attachments/assets/b196bc88-8696-4cb5-8fcb-c00f6442dc6a)


7. Open the newly created repository and explore its structure. 

## Task-2 Creating your first Codespace

You can create your first GitHub Codespace and learn how you can use Codespaces to work from anywhere from a browser. If you like more background information, please refer to the [GitHub Codespaces](https://docs.github.com/en/codespaces) pages on GitHub Docs.

### Steps to Follow
1. Navigate to your current repository
2. Under the repository name, use the  Code drop-down menu, and in the Codespaces tab, click Create codespace on main.

![image](https://github.com/user-attachments/assets/4f529c8b-e8bc-4162-aa53-2f50fe96dc46)


![image](https://github.com/user-attachments/assets/41535405-92ce-44a9-bfe7-10de42c81a8c)


## Task-3 Develop and push in a codespace
1. In the code folder open the readme.md file
2. Add the following in the readme.md file
```
Hello! From the codespace.
```
3. Save the file!
4. From the terminal run the following commands.
```
cd ..
git add *
git commit -m  "adding from codespace"
git push
```
5. You have now pushed code to your main repo! Codespace should look like this.

![image](https://github.com/user-attachments/assets/80104fc1-9057-43e5-9aa1-891b0f046614)


6. You can see the changes you have made in repo

![image](https://github.com/user-attachments/assets/71796170-0df0-4e06-bc38-b820640792e9)


## Outcome

By completing this exercise, you will:
- Understand how to create a repository.
- Be familiar with setting repository metadata such as name, description, and visibility.
- Explore the initial structure of a repository created.
- Creating your first Codespace
- Develop and push using codespace.
