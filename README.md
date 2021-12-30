# Workshop on Git and Project Management
<p align="center">
    <img alt="git-workshop-cover" src="https://user-images.githubusercontent.com/46085301/147738841-9c534b07-b7b0-40ae-989f-f37f78f277d8.png" />
</p>

## Prerequisites for the workshop 
- Install Git 
- Setup Github Account 
- Install VS Code

## Steps to be followed for the Workshop.

### Step 1: Setup
- [ ] Create folder named git-workshop on desktop
- [ ] Open the folder in vscode
- [ ] Configure git bash as default terminal
- [ ] Setup user configuration and then initialize the repo
    
  ```
      -- Configure user information for all local repositories
      $ git config --global user.name "[name]"

      -- Sets the name you want attached to your commit transactions
      $ git config --global user.email "[email address]"

      -- Initialize the repo
      $ git init
  ```
### Step 2: First Commit
- [ ] Create a markdown file named "README.md"
- [ ] Add few lines of dummy content
- [ ] Check status
- [ ] Stage the changes and commit with a message
    ``` 
        -- Check the status of the repo
        $ git status

        -- Stage single file
        $ git add [file]

        -- Stage all files with in the repo at once
        $ git add .

        -- Commit the changes
        $ git commit -m"[descriptive message]"

        -- To add and commit at once
        $ git commit -am"[descriptive message]"

        -- Check logs
        $ git log
        $ git log --oneline
    ```
### Step 3: Push to github Repo
- [ ] Create a github repo with default setting
- [ ] Add remote url of the repo and push
    ```
        -- Push an existing repository from the command line
        $ git remote add origin [repo url]
        $ git branch -M main
        $ git push -u origin main
    ```
- [ ] Setup configuration of authentication for github through vscode with default setting
    ```
        -- Optional Auth Setting after entering usename and password to cache for 1 hour
        $ git config --global credential.helper "cache --timeout=86400"
    ```
- [ ] Make some another changes and push
    ```
        $ git push

        -- Check some differences
        $ git diff
        -- Hit q to get out of the diff
    ```
- [ ] Try making some changes from github to readme file and then pull the changes
    ```
        $ git pull
    ```
- [ ] Try GUI based commiting and pushing changes
### Step 4: Ignoring the files
- [ ] Create a .gitignore file
- [ ] Add file names to gitignore to prevent from tracking
### Step 5: Branching
- [ ] Create a new branch named "add-feature-by-your_name" and checkout
    ```
        -- Check branches
        $ git branch

        -- Create a new branch 
        $ git branch "add-feature-by-your_name"

        -- Checkout to new branch
        $ git checkout [branch name]
    ```
- [ ] Make some changes, stage them and then push
    ```
        -- To add and commit at once
        $ git commit -am"[descriptive message]"

        -- Try git push. It will throw some fatal error with correct command
        $ git push --set-upstream origin [branch name]

        -- Delete merged branch
        $ git branch -d [branch name]

        -- Force delete
        $ git branch -fd [branch name]
    ```
### Step 6: Making pull Request and Merge
- [ ] Open github repo url and make pull request
- [ ] Add title, description and few lables (optional)
- [ ] Make some review if required
- [ ] Merge the branch and delete the branch if not required

### Step 7: Collaborating into the project
- [ ] Go to setting of the repo you are working
- [ ] Select manage access in the sidebar
- [ ] Add friends usernames with whom you want to collaborate
- [ ] Clone the repo (Not for the owner of the repo)
- [ ] Follow step 5 and 6 to create branch , make changes and merge
- [ ] Solve conflict if arised

### Step 8: Creating Issues
- [ ] Go to issues section of the repo and create a issue
- [ ] Describe the issue you want to create eg: bug request , feature request , etc
- [ ] Add assignee, label, etc for the issue
- [ ] Solve the issue by creating a PR that fixes the issue
- [ ] Setup templates for the issue ( optional) from setting of the repo

### Step 9: Creating Discussion Board
- [ ] Go to setting section of the repo
- [ ] Enable Dissussion option
- [ ] Go to Discussion Section
- [ ] Add few discussions
- [ ] See alternative way of discussing through slack

### Step 10: Setting up projects to track the progress
- [ ] Go to projects section and create a project named "progress board"
- [ ] Setup workflow
- [ ] Add few story for the backlogs
- [ ] Setup automation
- [ ] make some issuess wit pr and see the progress
- [ ] See alternatives eg: trello, jira.
 
### Step 11: Some of the extra features of Github
- [ ] Github Actions and it's importances
- [ ] Demonstration with few example
- [ ] Discuss about github pages
- [ ] See some concepts of CI/CD
- [ ] How testing and deployment works
- [ ] Writing readme files in readme.so

## 📚 RESOURCES:

1. Git Cheat Sheet: [https://training.github.com/downloads/github-git-cheat-sheet](https://training.github.com/downloads/github-git-cheat-sheet/)
2. Git Cheat Sheet by Mosh: [https://programmingwithmosh.com/wp-content/uploads/2020/09/Git-Cheat-Sheet.pdf](https://programmingwithmosh.com/wp-content/uploads/2020/09/Git-Cheat-Sheet.pdf)
3. Training Manual: [https://githubtraining.github.io/training-manual/](https://githubtraining.github.io/training-manual/#/01_getting_ready_for_class)
4. Git Downloads: [http://www.git-scm.com/downloads](http://www.git-scm.com/downloads)
5. VS Code Download: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)
## Authors

- [@bhimrazy](https://www.github.com/bhimrazy)


## License

[MIT](https://github.com/bhimrazy/Workshop-on-Git-and-Project-Management/blob/main/LICENSE)
