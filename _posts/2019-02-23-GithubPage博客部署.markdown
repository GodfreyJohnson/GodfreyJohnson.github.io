---
layout: post
title: GitHub Pages 博客环境搭建
date: 2019-02-23 15:32:24.000000000 +08:00
---

本文主要用于记录如何通过GitHub免费搭建自己的博客。

主要参考资料：https://www.jianshu.com/p/88c9e72978b4

总结主要步骤如下：

## mac下安装环境
```
sudo gem install jekyll
```

## 安装依赖 
```
bundle install
```

1.在这个过程中，若遇到没有安装bundle，需要先sudo gem install bundle
2.bundle install一直卡住没有打印任何信息，需要更新Gemfile中Source为：https://gems.ruby-china.com/

## 本地运行：http://127.0.0.1:4000/
```
bundle exec jekyll serve

```

## 把模板放到自己的仓库当中
```
git remote add -f $NAME $MY_REMOTE_REPO_URL
git add -u
git commit -m "**"
git push $NAME/master
```

