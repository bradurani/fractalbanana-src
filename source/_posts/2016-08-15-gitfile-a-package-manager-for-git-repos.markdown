---
layout: post
title: "Gitfile: A Package Manager for Git Repos"
date: 2016-08-15 23:38:53 -0700
comments: true
categories: [oss, gitfile, Go]
---

I just released the beta version of a new open-source project I put together
over the weekend. [Gitfile](https://github.com/bradurani/Gitfile) is a
lightweight package manager for installing and updating software from git repos.
It's great for installing odd things that live on GitHub and can't be installed
with typical package managers.
I built it because there are several things I wanted to include with my [dotfiles](https://github.com/bradurani/bradrc)
that can't be installed with brew, gem, npm, pip or any other common package
managers. They're things like [tmux plugins](https://github.com/thewtex/tmux-mem-cpu-load), [rbenv plugins](https://github.com/tpope/rbenv-ctags), and [zsh plugins](https://github.com/olivierverdier/zsh-git-prompt) that I want to
install automatically and update with a single command.  
Gitfile is written in [Go]("https://golang.org/") and I'd love contributions and
⭐️s. This was my first experience programming in Go. I haven't been that
interested in learning it because I'm so fond of the newer functional languages,
but this type of cross-platform command line app seemed like the right use case.
I got started in no time, and became productive more quickly than I ever have
with any other language. For me, it's a limited use case tool because it's
missing a lot of things I rely on when building big production apps. For
utilities like this though, I'd use it again.
