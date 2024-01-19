
## Branch, pull request, merge, rebase  


建立新的分支     
`git branch <new_branch_name>`

切換分支    
`git switch <branch_name>` 或
`git checkout <branch_name>`          

    也可以只用一行指令完成建立新的分支並且switch到那裡      
    >> git checkout -b <new_branch>

查看所有本地git branch  
`git branch`或
`git branch -a`  查看所有git branch 本地＋遠程


刪除分支   
`git branch -d <branch_name>`


Unstage     
`git reset <path>`

Remove whole thing and even the chached.       
`git rm --cached -r . `





Clone other 分支  
When you clone a remote repo, you will only see main branch, however, there are other branches hiding in your repository! See these using the -a flag

    $ git branch -a
    * main
      remotes/origin/HEAD
      remotes/origin/master
      remotes/origin/v1.0-stable
      remotes/origin/experimental

           
    $ git checkout experimental
    Branch experimental set up to track remote branch experimental from origin.
    Switched to a new branch 'experimental'

    
https://blog.csdn.net/shulianghan/article/details/18812279

or

添加遠程的某個分支   
`git branch  <branch_name_your_wanted_for local>  origin/<the_branch_from_remote> //origin 為遠程倉庫的匿名, 當然你也可以自訂義`

轉換帳戶:
For Mac: Go to KeyAccess >> Search for github >> delete all key access relate to github >> make a push using terminal command


開啟可視化工具   
`gitk --all`


You've deleted a remote feature branch on GitHub and it still appears when you run git branch -a locally, it may be due to the fact that Git keeps a local copy of remote branches as "remote-tracking branches." These remote-tracking branches are used to keep track of the state of branches on the remote repository.

To clean up these remote-tracking branches locally, you can use the following command:

`git fetch --prune`

The --prune option removes any remote-tracking branches that no longer exist on the remote. This should update your local repository with the current state of the remote branches.
