---
title: "Hugo 快速打造自己的部落格"
date: 2017-08-20T14:26:05+08:00
tags: [
    "test",
]
---
##前言
一直以來就很想要架個網站來玩一玩，原本是在Hexo、jekyll和Hugo之間選擇，後來因為選擇Hugo想說因為適用go語言寫的比較熟悉，於是來試試看。在Github上的Hugo開源專案有將近19000個star，使用人數非常的多。


Hugo是什麼呢？官網封面就寫著：
> Hugo is one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again.


以下環境皆以`Mac`電腦為準：
## 安裝Hugo

直接使用`Homebrew`安裝：
```
$ brew install hugo
```
接著把go下載下來，設定好`GOPATH`環境變量，並且得到原始碼
```
$ export GOPATH=$HOME/go
$ go get -v github.com/spf13/hugo
```
程式碼會下載到`$GOPATH/src`的目錄下，如果是下載binary則會在`$GOPATH/bin/`
如果需要更新所有Hugo的依賴library就增加參數`-u`：
```
go get -u -v github.com/spf13/hugo
```
## 生成網站
使用Hugo快速生成網站，例如希望生成到 /User/Mac/blog 的路徑
```
$ hugo new site /path/to/site
```
這樣就建立好目錄，移動到目錄位置：
```
cd /User/Mac/blog
```

結構大致上如下：
```
├ archetypes/
├ content/
├ layouts/
├ static/
└ config.toml
```


## 參考資源
[git 教學](https://git-scm.com/book/zh-tw/v1)  
[git submodule 新增、移除和使用](https://blog.longwin.com.tw/2015/05/git-submodule-add-remove-2015/)  
[使用Hugo搭建靜態站點](http://tonybai.com/2015/09/23/intro-of-gohugo/)  
[Hugo中文文檔](http://www.gohugo.org/doc/overview/configuration/)  
[Hugo静态网站生成器中文教程](http://nanshu.wang/post/2015-01-31/)  
[在 Github Pages 建立 Hugo 靜態網站](https://kaichu.io/2015/07/12/my-first-post/)
