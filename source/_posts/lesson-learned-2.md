---
title: Keep clear the difference between severity and priority
date: 2018-05-05 00:35:56
tags: lesson-learned
categories: sharing
---

In my early days in the software testing, I heard people talk about the severity and priority, but I don't seem to understand it yet. Have you encountered similar situation?

If yes, with me going around this post :)

#### What is Severity?
Whenever we refer to Severity of a defect, we are indicating the impact of the defect on the application's functionality. There are several levels to severity of a defect:
1. **Critical:** A defect causes the application to crash or corrupts data and blocks the user from performing any actions.
2. **Major:** A defect that causes one or more components of an application to fail but does not block the user from using other areas of the application.
3. **Minor:** A defect that affects the usability of the application but usually has a workaround.

#### What is Priority?
Whenever we refer to Priority of a defect, we are indicating the time frame within which the defect needs to be fixed/resolved. Like Severity, there are different levels to Priority as well:

<!-- A simple way, when you encounter a fatal error to your application, what is the first thing you think of? 

Right away, report bug to the programmer includes a notice that must be fixed immediately. That's why we need priority in bug reporting -->

1. **High:** The defect needs to be resolved within a working day. Because the defect is affecting the application or the product severely. The system cannot be used until the  repair has been done.
2. **Medium:** The defect should be resolved in the normal course of development activities. It can later be tested in another build or version. These defects do not crash the application.
2. **Low:** This defect does not affect functionality and has workarounds. It should therefore be fixed only after other important issues are resolved.

#### A few examples in fact
To easily visualize, let's take a look at the picture below. And I will take a few examples of the relationship between them.
![matrix](/congsang.github.com/images/lesson-learned/matrix.PNG)

**High Priority & High Severity:** An e-commercial site, purchase function does not work, high impact on business results, so high priority should be given.
**Low Severity & High Priority:** The logo or name of the company is not displayed on the website. It is important to fix the issue as soon as possible, although it may not cause a lot of damage.
**High Severity & Low Priority:** Error game, the game you have 60 level, at level 40 it crashed/failed to play. This is a serious error, but to achieve this level requires players to play a few months, so we can set the lower priority.
**Low Priority and Low Severity:** The privacy policy page take a long time to load. Not many people view the privacy policy page and slow loading doesn’t affect the customers much, so set to low priority.

#### Summary
Come to conclusion, we have things to remember:
- Severity refers to the impact or consequence of the bug. 
- Priority indicates when your company wants it fixed. 
