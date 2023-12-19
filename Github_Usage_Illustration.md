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
git push origin master **master要改成main**
git pull origin master **master要改成main**
```

![image-20231219220915893](C:\Users\MO\AppData\Roaming\Typora\typora-user-images\image-20231219220915893.png)

复制这段话到Git Bash中

### 更新文件

在使用 Git 向 GitHub 上推送文件后，如果本地文件发生更新，你可以通过以下步骤将这些更新同步到 GitHub 上：

1. **检查本地分支状态：**
   在你的项目目录中打开终端或命令行窗口，然后执行以下命令，查看本地分支的状态：
   ```bash
   git status
   ```

   这将显示有关本地仓库的当前状态，包括已修改的文件。

2. **添加已修改的文件到暂存区：**
   如果 `git status` 显示有已修改的文件，将这些文件添加到 Git 暂存区，使用以下命令：
   ```bash
   git add 文件名
   ```

   或者，如果想一次添加所有修改的文件，可以使用：
   ```bash
   git add .
   ```

3. **提交更改：**
   提交暂存区中的更改到本地仓库，执行以下命令：
   ```bash
   git commit -m "描述本次提交的信息"
   ```

4. **推送更改到 GitHub：**
   将本地的提交推送到 GitHub 上，执行以下命令：
   ```bash
   git push origin 分支名
   ```
   其中，`分支名` 是你要推送的分支的名称，通常是 `main` 或 `master`。

   如果是首次推送到 GitHub，可能需要提供 GitHub 账号和密码或者使用 SSH 密钥进行认证。

