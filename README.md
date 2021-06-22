# Github_commands
Basic Github commands and its brief explaination

### Initialize a Repository from existing code
	git init

### for checking the status of the repo
	git status

### add .gitignore file if u want to ignore a file from being tracked by git, you can use regular expressions as well

### Add files to staging area
	for individual file
		git add <file_name>
	for adding all
		git add --a

### Remove files from staging area
	for individual file
		git reset <file_name>
	for removing all 
		git reset --a

### To Commit with a message without opening defauld editor
	git commit -m "Initial commit"

### Clonning a remote repo
	git clone <url>
  
### see the differences between staged files and modified files
  git diff
  
### See the differences between staged files and previous latest commit files
  git diff --staged

### Pushing changes
	commit first
		git diff (To show the changes)
		git status (to show modified file)
		git add -A(add to staging area)
		git commit -m "Modified file"
	then push
		git pull origin master
		git push origin master

### Creating branch 
	git branch <name_of_branch> (to create a branch)
	git branch (to check the current working branch)
	git checkout <name_of_branch> (to switch to the branch)


### Pushing branch to remote
	git push -u origin <name_of_branch> 

### Merging a branch
	git checkout master (switch to master)
	git pull origin master
	git branch --merged (shows the merged branches)
	git merge <name_of_branch> (merge the branch) 
	git push origin master 

### Delete the branch
	git branch -d <name_of_branch> (to delete branch from local directory)
	git branch -a (to check branch in repo)
	git push origin --delete <name_of_branch> (to delete branch from repo)

### Rebase the branch
	git checkout <name_of_branch>(switch to branch)
	git rebase master (Changes the base of the branch to the lastest master commit)
  
 ### To check git version
	git --version

### to check git details 
	git config --list

### Need Help?
	git help <verb> OR
	git <verb> --help
  *eg. git config hep OR git help config*
