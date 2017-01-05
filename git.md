
## 设置user.email和user.name
当你安装Git后设置你的用户名称和e-mail地址，每次Git提交都会使用该信息。它被永远的嵌入到了你的提交中：
```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
重申一遍，你只需要做一次这个设置。如果你传递了 --global 选项，因为Git将总是会使用该信息来处理你在系统中所做的一切操作。如果你希望在一个特定的项目中使用不同的名称或e-mail地址，你可以在该项目中运行该命令而不要--global选项。

## 本地新建仓库，远程提交
```
echo "# notes" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:ishenry/notes.git
git push -u origin master
```
## push到远程仓库
```
git remote add origin git@github.com:ishenry/notes.git
git push -u origin master
```