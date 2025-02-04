# Developer_workflow GitHub Flow

## Objective
Learn how to configure branch protection policies for the default branch of a GitHub repository. This exercise ensures that changes to critical branches, such as main, meet certain requirements before being merged, enhancing code quality and repository integrity. Additionally, practice the **GitHub Flow** by collaboratively working on a application. This exercise focuses on creating issues for traceability, working with feature branches, modifying code, creating pull requests, and merging changes into the main branch.

## Prerequisites
1. **Git installed** on your local machine for managing the repository.

## Task-1: Enable Branch Protection Policy for the Default Branch

### Steps to Follow
1. Create a repository
2. Navigate to the created repository.
3. Go to the **Settings** tab of the repository on GitHub.

  ![image](https://github.com/user-attachments/assets/3cc1d399-437e-4129-a521-bf7e4b0cae4f)

   
4. Navigate to **Branches** under the **Code and automation** section and Click **Add classic branch protection rule**.

   ![image](https://github.com/user-attachments/assets/ecd71d2b-0c51-4797-b9bc-0cd5d1c0c43c)

   
5. Enter `main` as the branch name pattern (or your default branch name).

   ![image](https://github.com/user-attachments/assets/de9dda67-788e-4233-851c-1464c07fb166)

   
7. Select the following options:
   - **Require pull request reviews before merging.**
   - **Require review from Code Owners**
   - **Do not allow bypassing the above settings.**

![image](https://github.com/user-attachments/assets/2a0269db-affb-4f0f-856b-9e79c15a81ac)

     
8. Click on **Create** .

  ![image](https://github.com/user-attachments/assets/93d819c5-8bc4-4e32-ac39-84ef1eea05b1)
 


## Task-2: Practicing GitHub Flow

### Steps to Follow

### Create a GitHub Issue for Traceability

1. Navigate to the **Issues** tab of the repository.
   
   ![image](https://github.com/user-attachments/assets/743c5385-3b6c-45ce-97c2-d0a8e4271c77)


2. Click **New Issue**.

![image](https://github.com/user-attachments/assets/71cbf7ca-4500-4546-9f21-3ec84b302811)
   

4. Provide the following details:
   - **Title**: "Improve Index.cshtml File"
   - **Description**:

 ```
 `Index.cshtml` file in the `Tailspin.SpaceGame.Web/Views/Home` directory needs improvements to enhance code quality, performance, and maintainability.

## Task
### Code Cleanup
- [ ] Remove any commented-out code and unnecessary whitespace.
- [ ] Ensure consistent code formatting and indentation.

### Performance Optimization
- [ ] Optimize Razor syntax to improve rendering performance.
- [ ] Minimize the use of inline styles and scripts.

### Bug Fixes
- [ ] Identify and fix any existing bugs or issues in the file.
- [ ] Ensure the page works correctly across different browsers and devices.
 

```

![image](https://github.com/user-attachments/assets/a7cda0a2-8eef-47e0-8bfb-7868449cc386)


5. Assign the issue to yourself or a team member and click **Create**.

   ![image](https://github.com/user-attachments/assets/1f2d0981-b32a-446b-8956-288d49633b02)


### Outcome
By completing this exercise, you will:
- Understand how to configure branch protection rules to safeguard the default branch.
- Ensure that all changes undergo proper review and validation before merging.
- Maintain a high standard of code quality and repository security.
- Learn to create issues for traceability.
