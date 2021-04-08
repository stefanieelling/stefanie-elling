---
layout: post
title: Bug Exercises
subtitle: This Bugs Me
tags: [reading, reflection, open-source, bugs, zulip]
---
For today's blog, I discuss my experiences with exercises from Chapter 6 of Teaching Open Source and debugging a FOSS project. 

## Exercise 6.4 - Find the Oldest Bug
The oldest open Zulip [issue](https://github.com/zulip/zulip/issues/39) is "Installation Script Breaks Other Sites #39" and dates back to September 26, 2015. Zulip's installation seems to override configuration files and lacks an uninstallation script. This becomes a major issue if anything else is running on your server at the same time you install Zulip. Specifically, it clashes with nginx's main configuration. The only solution to this issue was adding a warning to a README file for users rather than fixing the actual problem. In another FOSS project I worked on, it was crucial to uninstall the installation script and I personally had to edit some of the configuration files. This issue means that Zulip is required to be installed in global scope rather than accounting for other softwares to be running at the same time. Personally, I am not equipped to solve this specific bug but hopefully someone will soon. 

## Exercise 6.5 - Create Your Bug Tracker Account
Before this class, I had already created a Github account and have worked on another FOSS project. Today, I created a Zulip account, installed the Dev environment, and joined the Zulip organization. This will allow me to claim and work on Zulip's open issues.

## Exercise 6.6 - Reproduce a Bug
For this exercise, I tried to recreate this [issue](https://github.com/zulip/zulip/issues/17169), titled "The Side-Bar Name Overlapping with Setting". I was able to recreate it in my own environment; however, I am unsure as to where this bug could be located. It seems like a simple html/css fix. One collaborator commented that this may be a 'normal' behavior only when the user's name is hovered while accessing the settings menu. Still, I find it to be odd and it should be fixed. 

## Exercise 6.7 - Bug Triage
For this exercise, I decided to 'triage' these five exercises: 
* [Issue #17156](https://github.com/zulip/zulip/issues/17156)
* [Issue #17147](https://github.com/zulip/zulip/issues/17147)
* [Issue #17059](https://github.com/zulip/zulip/issues/17059)
* [Issue #17037](https://github.com/zulip/zulip/issues/17037)
* [Issue #17009](https://github.com/zulip/zulip/issues/17009)

The textbook explains that a bug triage comes from the same approach used in medical fields, where professionals must determine which patients are prioritized. Thus, I have ranked these five issues based on their importance to Zulip. 
* [Problem inviting users #17147](https://github.com/zulip/zulip/issues/17147)
* [Add option to specify which users can create public and private streams separately. #17009](https://github.com/zulip/zulip/issues/17009)
* [widgets: Prevent edits to /poll and /todo messages. #17156](https://github.com/zulip/zulip/issues/17156)
* [Add "send test notification" button in settings #17059](https://github.com/zulip/zulip/issues/17059)
* [Add ability to search for custom emojis. #17037](https://github.com/zulip/zulip/issues/17037)

Mainly, I believed that the ability to invite users is essential to Zulip given that is a chat software. Thus, I think issue #17147 has the highest priority out of these five issues. Likewise, I believe that specifying which users can create public or private streams is very useful to organizations using Zulip and is a feature found in other softwares. It's important to differentiate the hierarchy and capabilities of group members within organizations, especially when dealing with managers and employees. The next two issues I believed are important in terms of testing and debugging the software, but I did not think they were as important to Zulip's regular users. And lastly, searching for custom emojis is a nice feature to have but I don't think it's essential in terms of Zulip's performance and user experience. 
