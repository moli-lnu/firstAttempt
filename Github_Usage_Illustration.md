# Git处体验及常用命令

1. 查看仓库的状态

   ```
   git status
   ```

2. 初始化Git仓库

   ```git init
   git init
   ```

3. 配置Github邮箱和用户名

   ```
   git config --global user.email "limo.karen.cs@gmail.com"
   git config --global user.name "moli-lnu"
   ```

4. 将hit.txt文件添加到Git仓库

   ```
   git add hit.txt
   ```

5. 将hit.txt文件提交到Git仓库

   ```
   git commit -m "text commit"
   ```

6. 打印Git仓库提交日志

   ```
   git log
   ```

7. 查看 Git 仓库的分支情况，创建a分支，并切换到a分支

   ```
   git branch
   git branch a
   git checkout a
   git checkout -b b
   ```

8. 合并命令

   ```
   git merge a
   ```

9. 删除分支

   ```
   git branch -d a
   git branch -D
   ```

10. 为当前分支添加标签

   ```
   git tag v1.0  //设置标签
   git tag 	//查看标签
   ```

# 利用 SSH 完成 Git 与 GitHub 的绑定

1. Git Bash中生成密钥

   ```
   ssh-keygen -t rsa
   ```

   

2. 添加SSK Key

   Github官网，头像，Settings，SSH and GPG keys, add *.pub文件中的内容

3. 验证绑定是否成功

   ```
   ssh -T git@github.com
   ```

   

   

# 通过Git将代码提交到GitHub

```
git push origin master
git pull origin master
```

![image-20231219220915893](C:\Users\MO\AppData\Roaming\Typora\typora-user-images\image-20231219220915893.png)

复制这段话到Git Bash中

