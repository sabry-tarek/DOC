
Git
----
----


- git help <span color= "#24f">***command*** </span>
- git config --global user.[name, email]
- git init
- git status
- git add <FileName> | git add .   <-->  git rm --cached [from index only] -r [recursive] .
- git commit -m "<Description>" -a [add] --amend [edit last commit]
- git log
- git diff | git diff head | git diff --staged | git diff <CommitNum> | git diff <CommitNum1><ComitNum2>
- git reset --soft [cancle last commit without cancel saved] --hard --hard head~1
- git branch | git branch <NewBranch> | git branch -d <BranchName> 
- git checkout <BranchName> | git checkout -b <NewBranchName> | git checkout <CommitID> /*must create new branch after this command to avoid the DETACHED HEAD*/ | git checkout <CommitID> -f
- git merge
- git satch <stach = cut for work directory> | git stach list | git satch apply [<StachName>] /*if you don't write StachID Git will use last stach*/ | git stach drop [<StachID>] | git stach pop <pop = apply + drop> [<StachID>]
- git remote -v | git remote add <ServerName> <ServerLink> | git remote remove <ServerName>
- git push -u <ServerName> <BranchName> | git push
- git pull <ServerName> <BranchName> | git pull
- git clone <ServerLink>

- git config alice.st status => var st = status ;

# .gitignore
# .gitadd
# Detached Head
-------------------------------------------------------------------------------------













