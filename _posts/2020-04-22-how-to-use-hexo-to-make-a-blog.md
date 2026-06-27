---
layout: post
title: How to use hexo to make a blog
date: 2020-04-22 20:04:49 +0800
last_modified_at: 2020-05-12 12:56:17 +0800
categories:
  - Web
tags:
  - hexo
permalink: /2020/04/22/How-to-use-hexo-to-make-a-blog/
---

## The Introduction for My First Blog

![Introduction screenshot](/images/2020-04-22-How-to-use-hexo-to-make-a-blog/1.png)

Choose **Slide Mode** in the top right sharing menu and hit **Preview** to see your slide.

---

For feature details please visit [https://github.com/hakimel/reveal.js/](https://github.com/hakimel/reveal.js/).

---

## The Preparing tools

**Operate system: Kali linux**

1. Git-it
2. Hexo
3. Vscode

---

## Install Git

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

Because of my linux system, the all of the installation progress will be used by terminal. Now we install git.

```shell
sudo apt-get install git
```

After the command running finish, you should check the git version to prove the git can work normally.

```shell
git --version
```

then the terminal will show this result.

![Git version output](/images/2020-04-22-How-to-use-hexo-to-make-a-blog/2.png)

---

## Install Hexo

Hexo is a fast, simple & powerful blog framework.

First you must install npm.

```shell
sudo apt-get install npm
```

Then you can use npm to insall hexo.

```shell
sudo npm install hexo-cli -g
```

Now you installed Hexo and you can check the version of Hexo.

```shell
hexo -v
```

![Hexo version output](/images/2020-04-22-How-to-use-hexo-to-make-a-blog/3.png)

---

## Install vscode

vscode is a powerful editor for any computer language.

First you should visit [https://code.visualstudio.com/](https://code.visualstudio.com/) and download the .deb file.

Now you should upgrade you permission.,

```shell
sudo chmod +x filename.deb
```

and install this application.

```shell
sudo dpkg -i filename.deb
```

After command running, you can run `code` in your terminal, the vscode will be start.

![Visual Studio Code](/images/2020-04-22-How-to-use-hexo-to-make-a-blog/4.png)

---

## Start your local server

First you need to create a folder to restore your local blog data. In here, I create this folder on my desktop.

```shell
mkdir Desktop/hexo
```

Next, you need to initialize your blog in this folder.

```shell
hexo init blog
```
