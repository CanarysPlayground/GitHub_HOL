# Create Pull Request and Merge Changes to Main Branch

### Task-1: Create a New Pull Request
1. Open your repository in GitHub.
2. Click the **Pull Requests** tab at the top of the repository view.  
3. Click **New Pull Request** to initiate the process.

![image](https://github.com/user-attachments/assets/91cdcb4f-395e-4cb5-8151-8933b7424264)
   
4. In the **Compare Changes** screen:
   - Select your working branch (`feature`) as the **source** branch.
   - Select the default branch (`main`) as the **target** branch.
     
5. GitHub will show a comparison of the changes. Ensure that all changes align with your expectations.

6. Click **Create Pull Request**.

   ![image](https://github.com/user-attachments/assets/c952877a-290d-499d-8df3-cbf76e2575dc)


 ### Task-2 Add Details to the Pull Request   

1. Provide a meaningful title and description for your pull request:
   - Clearly explain the purpose of the changes.
   - Mention any related tasks, tickets, or context to help reviewers understand the changes.
  
2. Add reviewers to your pull request:
   - Use the **Reviewers** option on the right-hand side to select team members.
   - Optionally, tag specific collaborators in the comments to provide additional guidance.

  ![image](https://github.com/user-attachments/assets/71a4f7fd-09cd-4f6d-b80d-1d20b2c8b675)

     
3. Notify reviewers about the pull request via comments, email, or team communication tools.
4. Reviewers will:
   - Click **Add Your Review**.

  ![image](https://github.com/user-attachments/assets/4ddf2de6-9698-4f79-bc5a-20332ef129ef)

     
   - Click **Review Changes**.
 
   ![image](https://github.com/user-attachments/assets/ce7c426f-6705-4365-8a29-a51d5368a2a8)
  

   - Provide feedback or approval:
     - Add comments or suggestions to the changes, if necessary.
     - Choose **Approve** to approve the pull request, and click **Submit Review**.
    
     ![image](https://github.com/user-attachments/assets/044356b7-5e8d-4a99-b541-f845e80c2b27)
 

> **Tip:** Incorporate feedback from reviewers promptly. You can push additional commits to the same branch, and GitHub will automatically include them in the pull request.

### Task-3 Merge Changes to the Target Branch
1. Once approved:
   - Click **Merge Pull Request**.

     ![image](https://github.com/user-attachments/assets/acf25f92-cd82-46c7-bff5-84c4032b0ea8)


   - Add a meaningful merge commit message if prompted.
   - Click **Confirm Merge**.
  
     ![image](https://github.com/user-attachments/assets/ce4b1b7d-8f61-46d9-91c3-a69a6c449c05)
 

2. You will see a **successfully merged** message indicating the process was completed.

    ![image](https://github.com/user-attachments/assets/64fe766b-13dd-49a9-88b4-b9199f4463e4)


3. Verify the Changes in the Main Branch
  - Navigate to the **main** branch in your repository.
  - Review the updated files and confirm that the changes have been successfully merged.

### Advanced Best Practices
- **Use Branch Naming Conventions:** Use consistent naming patterns, e.g., `feature` or `bugfix/fix-login-issue`.
- **Squash Commits:** Before merging, consider squashing commits to keep the main branch history clean and concise.
- **Enable Branch Protection Rules:** Set up branch protection rules to enforce approvals, passing checks, and linear history.
- **Review Automation:** Use GitHub Actions or bots to enforce code quality checks, run tests, or tag reviewers automatically.
- **Post-Merge Actions:** After merging:
  - Delete the feature branch to keep the repository tidy.
  - Inform stakeholders of the merge if needed.

> Following these advanced practices ensures a smooth collaboration process, minimizes conflicts, and maintains high code quality in your projects.
