---
layout: default
title: 2.2 Configure git
nav_order: 2
grand_parent: Tutorials
parent: 2. Starting with GitHub
has_children: false
---


# Configure git
{: .fs-8 }

Configure git on your system (one time only)
{: .fs-6 .fw-300 }

---

Now you have git installed, you need to set a few variables so git knows who you are and who is making changes to your documentation!

Open your command line application and enter the below, one line at a time (press return after each line). replace "Your Name" with your actual name...

```
git config --global user.name "Your Name"
git config --global user.email your-email-address@example.com
git config --global core.editor=atom --wait

```

You can then list the contents of your git config file using the command below, and check the above variables have been stored.

```
git config --list
```
