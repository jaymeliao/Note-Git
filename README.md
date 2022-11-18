
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

https://blog.csdn.net/shulianghan/article/details/18812279


添加遠程的某個分支   
`git branch  <branch_name_your_wanted_for local>  origin/<the_branch_from_remote> //origin 為遠程倉庫的匿名, 當然你也可以自訂義`
