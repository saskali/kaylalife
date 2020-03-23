---
title: "Interactive Commit Flow with Tig"
date: 2018-01-25T18:30:51+01:00
draft: false
categories: ["programming", "dev tools"]
---

#### Minimal tig keybindings to make the most out of your commit flow.

It was at my first programming internship that one of my collegues showed me how to use tig. It is a text-mode interface that offers a more interactive and flexibel way of developing  compared to using git with the command line only. I have been using it ever since and I feel more productive and in control of my commit flow. Since a few people have kept asking me about it, I decided to write this blog post. 

Tig has a lot of features most of which I will ignore. I am going to describe the minimal amount of steps to make tig part of your everyday workflow. I find it most useful for selectively deciding which changes I want to make part of my commit and which ones I want to ignore. 


### How can I use tig?

To get tig setup on your machine, follow [these](https://github.com/jonas/tig/blob/master/INSTALL.adoc) installation instructions. For Ubuntu users: 

    sudo apt install tig

For Mac users: 

    brew install tig --HEAD

Equivalent of `git status`

    tig status

Show my commit history

	tig --all

### Navigation

There are six essential keys for basic navigating through tig.

key           | action                        |
--------------|-------------------------------|
↑ ↓           | navigation to select file     |
j / k         | navigation within file        |
enter         | open changes of selected file |
q             | go back                       | 

### Choose Code to Commit 

These three keybindings are the ones to remember for deciding what will be part of your commit. 

key           | action                                               |
--------------|------------------------------------------------------|
u             | move code between staging area and working directory |
!             | discard changes                                      |
\\            | make a new split in the code                         |

### I want to learn more about tig 

Yes, tig can do much more. If you're simply looking for a more interactive way of making commits, these simple steps can get you to a more efficient work flow. For more information, check out this [cheatsheet](https://devhints.io/tig) and find more detailed information on [tig's website](https://jonas.github.io/tig/).

