# Create CI/CD workflow

### Task-1 Create a new CI Workflow
1. In the `.github/workflows` directory, create a file named 'space-game.yml'
2. Copy the following YAML contents into the 'space-game.yml' file:

```
name: GitHub Actions CI/CD
on:
  push:
   branches: main
  pull_request:
   branches: main
   
  workflow_dispatch:
  
jobs:
  Build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run a one-line script
        run: echo Hello, world!
      
      - name: Upload a Build Artifact
        uses: actions/upload-artifact@v4
        with:
         name: Artifact
         path: ${{github.workspace}}/*  
     
```

3. Committing the workflow file to a branch in your repository triggers the push event and runs your workflow

4. You can see the live logs of the workflow and the generated artifact.

  ![image](https://github.com/user-attachments/assets/49d66f85-28da-48dd-a17b-4ef592c083df)
 

### Task-2 Create a Dev Evironment

1. On GitHub, navigate to the main page of the repository.
2. Click `Settings` 
3. In the left sidebar, click `Environments`
4. Click `New Environment`
5. In the `Name*` field type `Dev`
6. Click `Configure Environment`
7. Click `Save Protection rules`

### Task-3 Create a Production Evironment

1. In the left sidebar, click `Environments`
2. Click `New Environment`
3. In the `Name*` field type `Production`
4. Click `Configure Environment`
5. Select `Required Reviewers` checkbox
6. Add yourself as a review
7. Click `Save Protection rules`

### Tasak-4 Add the following workflow

1. On GitHub, navigate to the main page of the repository.
2. Open file `.github/workflows/space-game.yml`
4. Edit workflow file `.github/workflows/space-game.yml`
5. Paste in the following code:
```
###################################################################
#Deploy action

DeployToDev:
    runs-on: windows-latest
    needs: Build
    environment: Dev
        
    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:
      # Runs a single command using the runners shell
      - name: Deploying To Dev for ${{ inputs.ghhandle }}!
        run: "echo I just deployed to Dev"

  DeployToProd:
    runs-on: windows-latest
    needs: DeployToDev
    environment: Production
    
    steps:
      - name: Deploying To Production for ${{ inputs.ghhandle }}!
        run: "echo I just deployed to Production"
  
###################################################################

```

![image](https://github.com/user-attachments/assets/6dba6d4c-0924-48ba-abc0-c7fb6fc250e5)

