# Creating your first Action Workflow

In this hands-on lab your will create your first GitHub Action Workflow and learn how you can use Actions to automate tasks in your software development lifecycle. If you like more background information, please refer to the [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions) pages on GitHub Docs. Good luck! 👍

> Before you start with this lab, please remove the branch rule, so you can commit to the main branch without a pull request to speed up the process :smirk:

This hands on lab consists of the following steps:
- [Enabling Actions](#enabling-github-actions)
- [Creating the workflow](#creating-the-workflow)
- [Viewing your workflow results](#viewing-your-workflow-results)
- [Only trigger workflow when a change is made to the website](#only-trigger-workflow-when-a-change-is-made-to-the-website)
- [Only trigger workflow on new issue created](#only-trigger-workflow-on-new-issue-created)
- [Create a Matrix build for release and debug](#create-a-matrix-build-for-release-and-debug)

## Enabling Github Actions
1. Work inside your current repository `Martixcomsec-training/attendee-<your-github-handle>`
2. Go to Settings -> Actions -> General
3. Check 'Allow all actions and reusable workflows', and click save

## Creating the workflow
1. Work inside your current repository `Martixcomsec-training/attendee-<your-github-handle>`
2. Create a `.github/workflows` directory in your repository on GitHub if this directory does not already exist.
3. In the `.github/workflows` directory, create a file named `github-actions-demo.yml`.
4. Copy the following YAML contents into the `github-actions-demo.yml` file:
```YAML
name: GitHub Actions Demo
on: [push]
jobs:
  Explore-GitHub-Actions:
    runs-on: ubuntu-latest
    steps:
      - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
      - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
      - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
      - name: Check out repository code
        uses: actions/checkout@v3
      - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner."
      - run: echo "🖥️ The workflow is now ready to test your code on the runner."
      - name: List files in the repository
        run: |
          ls ${{ github.workspace }}
      - run: echo "🍏 This job's status is ${{ job.status }}."
```
5. Scroll to the bottom of the page and select `Create` a new branch for this commit and start a pull request. Then, to create a pull request, click `Propose new file`.
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-commit-new-file.png)

Committing the workflow file to a branch in your repository triggers the push event and runs your workflow.

## Viewing your workflow results
1. On GitHub, navigate to the main page of the repository.
2. Under your repository name, click `Actions`.
![](https://docs.github.com/assets/images/help/repository/actions-tab.png)

3. In the left sidebar, click the workflow you want to see.
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-workflow-sidebar.png)

4. From the list of workflow runs, click the name of the run you want to see.
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-run-name.png)

5. Under `Jobs` , click the `Explore-GitHub-Actions` job.
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-job.png)

6. The log shows you how each of the steps was processed. Expand any of the steps to view its details.
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-logs.png)

For example, you can see the list of files in your repository:
![](https://docs.github.com/assets/images/help/repository/actions-quickstart-log-detail.png)


## Only trigger workflow when a change is made to the website

See: [Workflow syntax for github actions - on push/pull - request paths.](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestpaths)
```
name: GitHub Actions Demo
on:
  push:
    paths:
    - 'code/src/AttendeeSite/**/*'
jobs:

...
...
```

## Only trigger workflow on new issue created

See: [Webhook events and payloads - Issues](https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#issues)
```
...
...

on:
  issues:
    types: [opened]

...
...
```

## Create a Matrix build for release and debug
See: [Workflow Syntax - Jobs - Matrix Strategy](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idstrategymatrix)

```
...
...

Explore-GitHub-Actions:
    runs-on: ubuntu-latest  
    strategy:
      matrix:
        configuration: [debug, release]
    steps:
    - run: echo "🔧 Building the configuration ${{ matrix.configuration }}."

...
...
```

