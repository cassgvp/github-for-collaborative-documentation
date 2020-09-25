---
layout: default
title: 2.4 Basic git commands
nav_order: 4
grand_parent: Tutorials
parent: 2. Starting with GitHub
has_children: false
---

# Basic git commands
{: .fs-8 }

Use these commands to do 90% of your work
{: .fs-6 .fw-300 }

---

## I am NOT a git wizard

Practicing some radical transparency here, folks 😉. I can do enough git to get buy (I also like hearing myself say "git" in a Southern American accent where it sounds just like "get" to me), and just about fix things when they break. Every time I break something, I learn a little more, and that works for me 😊. Seems I'm not alone.

![xkcd-git](https://imgs.xkcd.com/comics/git.png)

While I think it is SUPER cool to know everything about git and understand all the stuff, I totally respect that not everyone has that much time available to learn all the new things, and to expect everyone to be a wizard at something before they can participate make for a very exclusive and unwelcoming community.

In the spirit of inclusivity, I'm going to show you the git commands I know, and then you too will be able to do just enough git to get by, and make use of this excellent resource in a way which works for you.

## The three(ish) stages of adding to your repository online

For reasons which are better explained by someone who understands how git works more completely than I do, there are three stages (commands) required to transfer your local changes to your online repository for others to see.

**All of this happens in your command line application**. To use the commands, you'll be sat in the directory which contains your code which is being tracked by git, and entering the commands from there.

While entering all these commands, keep an eye on the messages appearing in your command line application. They may look incomprehensible at first, but with a little practice and patience you be able to identify the key parts and work out what is happening or going wrong!

### 0. Ask git to tell you what has changed

I love `git status`. Sometimes I know exactly what I've changed, and sometimes I'll have been jumping all over the place changing multiple files. Before I upload any changes, I'll usually run the `git status` command to remind me of what files I've been working on, so I can write a sensible commit message (see below)

### 1. Add

`git add your-file-name`

Tell git to "add" the file which you have changed (here called *your-file-name*)" to a staging area, ready to be updated. You can add individual files buy repeating the line with each file name, or you can use `git add .` to add everything which has been changed. I use this a lot.

### 2. Commit

Once you've added files to the staging area, you are ready to "commit" these to your repository. When we do this, we'll add a message for yourselves and our contributors explaining what changes we made in those files. The `-m` "flag" in the command below denotes that what follows will be your commit message.

`git commit -m "fixed broken link"`

Here I'm saying that the change I made in the file added above was to fix a broken link.

Your commit message can be anything you like, but there are some [best practice guides you can follow](https://chris.beams.io/posts/git-commit/) if you want to get deep. I like to keep it short and meaningful. In essence, you should be able to look back at your commit log and get an idea of the important things you did at each stage, incase you need to come back to a specific point later.

### 3. Push

You've added files to your staging area, you are committed to uploading them, now you actually need to **push** them to your repository. This one is easy.

`git push`

Everything you have added will be uploaded ("pushed") to your repository.

At this point (especially if it is a bit load of changes I'm uploading) I'll often skip excitedly over to my online repository and have a look at my commit and the file changes. It's almost as if I don't trust the magic!?! 😉




## The one stage of pulling a copy of your online repository
