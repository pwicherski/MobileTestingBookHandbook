---
description: v1.0
---

# Test Plan

### Introduction

The Test Plan has been created to communicate the test approach to team members. It includes the objectives, scope, schedule, risks and approach. This document will clearly identify what the test deliverables will be and what is deemed in and out of scope.

As the team works with the product they will define the needs for the second phase.

#### Team communication

All communication is performed though Slack and Github issues.

#### Objectives

The 1.0 phase will focus on manual testing for now and then we'll migrate to automation in the future. Preferably in next major test plan update, next app release will folow.

App milestones for 1.0:  
[https://github.com/WorldHealthOrganization/app/milestone/4](https://github.com/WorldHealthOrganization/app/milestone/4)

#### Application architecture

Application is written in Flutter framework. We need to have this in mind and choose appropriate tools and approach.

We're supporting Android and iOS mobile operating systems.

* IOS from 8 to 13
* Android from 4.1\(API 16\) to 10.0 \(API 29\);

## Plan

_"Next steps"_ are non-essential parts for this release, but it would be nice to have if we will have enough time and resource to do them. We will focus on them in next phase.

### Manual tests

We should focus on all user interface elements, hand washing animation in "Protect Yourself".

### Automated checks

We plan to use Firebase Robo test checks for now, and add UI intergration tests in the second phase.

We can also use cloud device labs as a support in performing various test types.

### Compatibility with Device Hardware

#### Different screen sizes;

#### Different screen resolutions;

#### Low/mid/high internet speed;

#### App permissions;

#### Next steps:

* Gestures;
* Touch areas;
* Device temperature;
* Higher data package loss;
* Switching between different types of networks;
* Low memory;
* Switching between applications;

### Compatibility with Device Software

#### Sending, receiving and opening app notifications;



#### Installability testing

#### Stress testing

#### Security testing

#### Performance testing

#### Usability testing

#### Database testing

#### Accessibility testing

* Check screen readers;
* Check high contrast colors;
* Check black and white screen colors;

### To test

In manual testing we should focus on all user interface elements, hand washing animation in "Protect Yourself".

### Test procedures

### Tools

### Risks

#### We don't exacly know what devices our users will use.

That's our main risk. We need to assume that they could use anything ranging from Samsung Galaxy S3 \(Android 4.3\) and iPhone 4s \(iOS 9.3.5\) to Samsung Galaxy Folder 2 \(3.8" screen\), Samsung Galaxy View SM-760 \(18.4" screen\) and Infinix Zero 5 Pro \(with Mediatek MT6757CD Helio P20 CPU\) ending with Xiaomi Redmi K30 Pro \(2020 release\).

We must deal with multiple device types, OS versions, screen sizes, quality of display and many more. 











