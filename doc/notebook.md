# 常见问题汇总

## 本地文件夹关联远程仓库时出错

> **问题描述**

按照如下流程将本地文件夹关联到远程仓库

```zsh
#初始化git仓库
git init  
#添加所有文件
git add .  
#添加提交信息
git commit -m '提交信息' 
#添加远程仓库地址
git remote add origin remote_git_url 
#拉取远程仓库所有内容,并将所有非空文件提交
git pull --rebase origin master 
#将此次提交推送至远程仓库
git push origin master 
```

在最后一步出现如下错误：

```zsh
(base) iiixv@IIIXVdeMacBook-Air PiggyMetrics % git push origin master
error: src refspec master does not match any
error: failed to push some refs to 'github.com:manjixx/piggymetrics.git'****
```

> **解决方案**

[解决方案](https://www.freecodecamp.org/news/error-src-refspec-master-does-not-match-any-how-to-fix-in-git/)