# Basic Rules: #
- If you are going to edit the code, create a new branch and work there so the main code is not disrupted
- When making a commit, state the specific change that has been made so other people know what it is
- If you want to, feel free to ask other people to review your code through the Github (they can access your branches)
- When you are done with all your code, and it has been committed, push the code and then delete the branch that you were working on

## Introductory Rule ##

Just to make sure that you can edit the code and write pull requests, create a new branch and write something silly in test.txt in the SEPP-CW2-Task-5 File and then make a pull request for it

# Introduction to Git branches #

The main branch you are working on is called ```main```. If you are not working on anything this should be where you are at

## Updating your own code ##

When other people have updated code, use 

```
git checkout main (If you are not on the main branch)
git pull origin main
```

To update your code to the current version

## Working with your own branches ##

To create a working branch, use the following:

```
git checkout -b your_branch
```

This will directly put you in a new branch with all the pre-existing code

When you are ready to push your code to the main repository, use the following:

```
git add .
git commit -m "Add Stripe checkout session creation"
git push
```

Copy, paste and run the following command, which will automatically create a pull request others can see

It should look something like the below:
```
git push --set-upstream origin test_branch
```

Afterwards, it will provide a link to a pull request like this: https://github.com/NathanielCC/SEPP-CW2-CW3/pull/new/test_branch

Click on it and go and review your code. Afterwards, if there are no issues, click merge to go ahead and add it to the main files.

## Deleting obsolete branches ##

When working with branches, avoiding branches to solved problems is important. 

First make sure you are in the main branch, using the following command:

```
git checkout main 
```

Then, use the following command:

```
git branch -d branch_name
```

This should get rid of any obsolete branches that aren't being used anymore

## Resolving Conflicts ## 

Refer to this link:

https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line

