Some things about working on Github with other people:
- If you are going to edit the code, create a new branch and work there so the main code is not disrupted
- When making a commit, state the specific change that has been made so other people know what it is
- If you want to, feel free to ask other people to review your code
- When you are done with all your code, and it has been committed, push the code and then delete the branch that you were working on

The main branch you are working on is called **main**. If you are not working on anything this should be where you are at

When other people have updated code, use 

**git switch main** (If you are not on the main branch)
**git pull origin main**

To update your code to the current version

To create a working branch, use the following:

**git checkout -b your_branch**

This will directly put you in a new branch with all the pre-existing code

When you are ready to push your code to the main repository, use the following: