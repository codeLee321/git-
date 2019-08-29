# Git使用总结

### 远程仓库创建
```sh
$ git init  								#创建本地仓库
$ echo "# git-summary" >> README.md  					#创建说明
$ git add README.md 							#添加本地文件
$ git commit -m "first commit"   					#添加提交说明
$ git remote add origin https://github.com/codeLee321/git-summary.git 	#关联远程仓库
$ git push --set-upstream origin master  				#将本地文件推向远程仓库
$ git push -u origin master 						#强推
```
### 分支管理

##
```sh
$ git checkout -b dev 							#-b参数表示创建并切换分支
$ git branch								#查看当前分支
$ git checkout master							#切到master分支
$ git merge dev								#将dev分支合并到当前分支
$ git branch -d dev 							#删除dev分支

#高版本git提供switch
$ git switch -c dev							#创建并切换分支
$ git switch master							#切到master分支
$ git status								#查看当前分支状态以及文件冲突
$ git log --graph --pretty=oneline --abbrev-commit			#查看合并记录
$ git merge --no-ff -m "merge with no-ff" dev				#合并禁用Fast forward
``
`
