# git入门

## 1.git是什么

- 一个分布式版本控制的软件

## 2.为什么要做版本控制

- 要保留之前所有的版本，以便回滚和修改

## 3.使用git管理

- 进入要管理的目录、
- 执行初始化命令，即：让git管理当前目录

```
git init	
```

- 检测当前目录下文件的状态

```
git status
注：新增的文件和修改过后的文件都是红色
```

- 管理指定文件（红变绿）

```
git add 文件名          -管理单个文件
git add .                      -管理所有未管理的文件
```

- 个人信息配置：用户名、邮箱

```
git config --global user.email "you@example.com" 
git config --global user.name "Your Name"
```

- 生成版本

```
git commit -m '描述信息'
```

- 查看版本记录

```
git log
```

- 回滚

  1.回滚至之前的版本

```
git log
git reset  --hard  版本号
```

​		2.回滚至之后的版本

```
git reflog
git reset  --hard  版本号
```

## 4.git常用命令小总结

```
git add 										-管理单个文件
git add .                      					-管理所有未管理的文件
git commit	'描述信息'			-生成版本					-
git reset HEAD                          -将暂存区的返回为工作区
git checkout                             -将工作区的返回为未管理的文件
git reset --hard 版本号          -将版本库的返回为工作区
```

## 5.分支

- 查看 分支

```
git branch
```

- 创建分支

```
git branch 分支名
```

- 切换分支

```
git checkout 分支名
```

- 合并分支（可能会产生冲突）

```
git merge 分支名
注意：切换分支再合并
```

- 删除分支

```
git  branch -d 分支名
```

## 6.github

- 给远程仓库取名

```
git remote add 仓库名 仓库网址
```

- 将本地代码推送到远程仓库

```
git push -u 仓库名 分支名
注意：-u可写可不写
```

- 克隆远程仓库代码（第一次获取代码）

```
git clone 仓库地址 （内部已实现取名）
```

- 获取远程仓库分支

```
git pull 仓库名 分支名
```

- 查看文件

```
cat 文件名
```

