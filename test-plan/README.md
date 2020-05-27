---
For release: v1.0
---

# Test Plan

### Introduction

The Test Plan has been created to communicate the test approach to team members. It includes the objectives, scope, schedule, risks and approach. This document will clearly identify what the test deliverables will be and what is deemed in and out of scope.

As the team works with the product they will define the needs for the second phase.

### Team communication

All communication is performed though Slack and Github issues.

### Objectives

The 1.0 phase will focus on manual testing for now and then we'll migrate to automation in the future. Preferably in next major test plan update, next app release will folow.

App milestones for 1.0:  
[https://github.com/WorldHealthOrganization/app/milestone/4](https://github.com/WorldHealthOrganization/app/milestone/4)

### Application architecture

Application is written in Flutter framework. We need to have this in mind and choose appropriate tools and approach.

We're supporting Android and iOS mobile operating systems.

* IOS from 8 to 13
* Android from 4.1\(API 16\) to 10.0 \(API 29\);

## Plan

### Manual tests

#### Scope

In manual testing we should focus on all user interface elements, hand washing animation in "Protect Yourself".

#### Examples of configurations to focus on;

* Android GO.
* Older devices such as Galaxy S3 and iPhone 4s.
* Smaller screen devices - iPhone 5.
* Big screens - big tablets such as SM-T670 18.4".
* Big screen with smaller resolution - iPhone XR.
* Xiadomi devices.

### Automated checks

We plan to use Firebase Robo test checks for now, and add UI intergration tests in the second phase.

We can also use cloud device labs as a support in performing various test types.

### Compatibility with Device Hardware

#### Different screen sizes and resolutions;

* The app scales all user interface elements according to current screen density and size.
* User interface elements do not overlap.
* Usability or touch issues do not occur. 
* There is no problematic shrinkage of images because of high dpi/ppi.

#### App permissions;

* The app is able to work with reduced permissions. It asks the user to grant these permissions and does not fail in an unexplained manner.
* Permissions are only requested for the resources which are relevant to the app’s functionality.
* The app functionality responds correctly if a permission is withdrawn or rejected.

### Compatibility with Device Software

#### Sending, receiving and opening app notifications;

* The correct handling of notifications received when the app is in the foreground or background, especially under low battery conditions.

#### User Preferences

* Users can amend typical preference options such as sound, brightness, network, power save mode, date and time, time zone, languages, access type and notifications.
* The apps adhere to the set preferences by behaving accordingly.

#### Interoperability

* Various system overlays made by manufacturers
  * Samsung TouchWiz
  * Samsung OneUI
  * Huawei EMUI
  * HTC Sense
  * LG UX
  * Google Pixel UI
  * Sony Xperia UI

### Various Connectivity Methods

#### Low/mid/high internet speed;

* How app behavies without internet.
* How app behavies with slow internet.
* Correct app functionality with different connectivity modes.
* Switching between modes does not cause any unexpected behavior or data loss.
* Clear information is given to the user if functionality is restricted due to limited or no network connection or if bandwidth is low. The message should state the limitations and their reasons.

### Test Types to perform

#### Installability testing

* Is the installation process clear.
* Re-installation.
* Uninstall.

#### Stress testing

* Low disk space.
* High CPU-usage.
* Device with slow CPU.

#### Performance testing

* Check slow and older devices.

#### Usability testing

* Be self-explanatory and intuitive.
* Allow user mistakes.
* Be consistent in wording and behavior. 
* Make needed information visible and reachable in each screen size and type.

#### Accessibility testing

* Check screen readers;
* Check high contrast colors;
* Check black and white screen colors;

### Test procedures

#### Coverage

After performing tests fill Device Coverage Sheet, so we could estimate our Device/OS/Overlay coverage.

#### Bug bash

Bug bash will have their own procedure which will be send to invited users.

### Risks

#### We don't exacly know what devices our users will use.

That's our main risk. We need to assume that they could use anything ranging from Samsung Galaxy S3 \(Android 4.3\) and iPhone 4s \(iOS 9.3.5\) to Samsung Galaxy Folder 2 \(3.8" screen\), Samsung Galaxy View SM-760 \(18.4" screen\) and Infinix Zero 5 Pro \(with Mediatek MT6757CD Helio P20 CPU\) ending with Xiaomi Redmi K30 Pro \(2020 release\).

We must deal with multiple device types, OS versions, screen sizes, quality of display and many more.

