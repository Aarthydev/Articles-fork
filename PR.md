[GitHub Repository Link](https://github.com/techeazy-consulting/lmds)


### Step 1: Accept Collaborator Request and Clone GitHub Repository

- You have received an invitation to join a GitHub repository in your email. Please accept the invitation.

  ![email_collabator_invitation](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2FupadtedGitHubPR%2Femail_collabator_invitation.png?alt=media&token=cfbe8e45-c03c-4e13-9bc0-3c4e299f696e)

  ![accept_invitation](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2FupadtedGitHubPR%2Faccept_invitation.png?alt=media&token=4275fd81-5295-4b9f-bc99-c66a854bfc0f)

  ![github_home_page](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2FupadtedGitHubPR%2Fgithub_home_page.png?alt=media&token=044ac245-6cdf-452f-9c4e-d8a104f09ff4)


- Clone the GitHub repository using the command:

  `git clone <github repo url>`

  In our case:

  `git clone https://github.com/techeazy-consulting/lmds.git`


- Navigate to the local directory, open Git Bash or CMD in this directory, and execute the command above.

  ![clone_github_repo](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2FupadtedGitHubPR%2Fclone_github_repo.png?alt=media&token=94587cf0-ae22-4e48-a230-90d6eca94ac5)

- Now you have successfully cloned the GitHub repository. You can open Eclipse IDE in this directory and start working.

---


### Step 2: Create Pull Request on existing GitHub repository


- Go to local repository and **Create a new branch** using the command:

  ```bash
  git checkout -b "<branch-name>"
  ```

  ![created-new-branch-pr](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fcreated-new-branch-pr.png?alt=media&token=4fb488d2-3797-4d2e-b466-13a8a97dad95)

- Now you are switched to the new branch. Let's suppose we created **working-branch**. You can work on this branch and make code changes.
- Let's suppose we created a simple entity in our project. So changes happened.
- Again, stage and commit the changes, then push the code to the new branch. In our case, it is **working-branch**:

  ```bash
  git add .
  git commit -m "created user entity"
  git push origin working-branch
  ```

  ![stage-commit-push-pr](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fstage-commit-push-pr.png?alt=media&token=a8c6ff80-c903-4fa8-b976-82f0fd4e0cb7)

- You can see on the GitHub repository, the new branch is created (`working-branch`).

  ![working-branch-on-github](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fworking-branch-on-github.png?alt=media&token=f6138e41-74a9-4583-a7c9-e5123aa22821)

- **Click on the "Pull request" option.**

  ![pull-request-option](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fpull-request-option.png?alt=media&token=43d87b4c-0aab-4deb-9505-09267820ab74)

- **Click on the "New Pull request" option.**

  ![new-pull-request-option](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fnew-pull-request-option.png?alt=media&token=dc3fa3d9-c035-4bc4-b76a-d9be2769750b)

- Choose `base: master` and `compare: <created-branch-name>`. In our case, it is `base: master` and `compare: working-branch`. Then click on the "Create pull request" button.

  ![choose-branch-create-pr](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fchoose-branch-create-pr.png?alt=media&token=a404f7a3-f5d8-4a67-a68c-0a134a23a0d5)

- On the next page, add a title and description for the Pull Request.
- Also, click on the "Reviewer" option (settings button) and choose a collaborator (the person you want to show the changes to). For this, you need to have added the collaborator to your GitHub repository.
- Click on "Create pull request."

  ![title-description-pr](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Ftitle-description-pr.png?alt=media&token=b26ddd18-5bf5-4d69-bf4e-96e50bbb0fa1)

- On the next page, click on "Merge pull request" and then confirm the merge.

  ![merged-pull-request](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fmerged-pull-request.png?alt=media&token=6338ada2-91f1-40f1-81d1-b1bb4e954ade)

- You can see that you have successfully merged the desired branch into the master branch. An email notification is also sent to the selected reviewer (collaborator).

  ![master-branch-merged-completed](https://firebasestorage.googleapis.com/v0/b/techeazy-consulting-blog.appspot.com/o/Blog%20Images%2Fmaster-branch-meged-completed.png?alt=media&token=40a9200a-75f1-4121-8b10-acb2f0a14ea5)
