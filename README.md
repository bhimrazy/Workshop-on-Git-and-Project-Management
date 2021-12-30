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
- [ ] Setup user configuration
    
  ```
      -- Configure user information for all local repositories
      $ git config --global user.name "[name]"

      -- Sets the name you want attached to your commit transactions
      $ git config --global user.email "[email address]"
  ```
### Step 2: First Commit
- [ ] Create a markdown file named "README.md"
- [ ] Add few lines of dummy content
- [ ] Check status
- [ ] Stage the changes and commit with a message
    ``` 
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
- [ ] Setup configuration of authentication for vscode with default setting
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
