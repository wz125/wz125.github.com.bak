---
layout: post
title: 'debian-xfce-install'
category: blog
tags: [debian]
---


Install Xfce in an already installed system  
--

To get a bare minimum base install of X, do:  
    `aptitude install xorg`  
    `aptitude install xfce4-goodies`  
    `aptitude install xfce4`  
This will install a meta package, which will install the core XFCE modules and scripts to get it to work.
There are many useful utilities that come with XFCE, to install these:
    `aptitude install xfce4-goodies`

Run Xfce
--

2.1 For GDM/KDM choose xfce4-session.

2.2 For startx add in file ~/.xinitrc:
    `exec ck-launch-session startxfce4`

2.3 For slim boot session in /etc/slim.conf:
    login_cmd exec ck-launch-session /bin/bash -login /etc/X11/Xsession %session

2.4 You also can install lightdm/xdm to login in start Xfce.

引用：
--
  http://wiki.debian.org/Xfce

