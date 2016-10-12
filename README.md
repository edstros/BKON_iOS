### Add BKON Mobile SDK to a new or existing Swift project

#### Introduction
The [BKON Mobile SDK](https://www.phy.net/sdk/physical-web-sdk-ios/) is a powerful tool for detecting, and interacting with both iBeacon and Physical Web beacons in a single application.

[BKON](https://bkon.com/) is a company based in Nashville, TN., producing hardware and software for the physical web.

#### Requirements

iBeacon technology, depends on Core Location, support which was added in iOS 7.  Although Physical Web beaons to not depend on this, if you would like to support both, please target iOS 7 or later with your application.

This guide will not go through the process of setting up an iOS application project using Swift, however this guide can be used on any new or existing Swift project.

#### Guide

Adding the BKON Mobile SDK to an existing Swift project requires a few simple steps.  Because the BKON Mobile SDK is written in Objective-C, it will require adding a bridging header to your project.

First, let's add the BKON SDK to our project.  Navigate to File -> Add Files to "PROJ_NAME"... and select the PhySdk.framework file which can be found in your downloaded copy of the BKON Mobile SDK:

![](http://i.imgur.com/uP6MmbV.png)
![](http://i.imgur.com/8exSQxO.png)

Next, we will need to add a bridging header file to our project, to allow us to use the BKON Mobile Objective-C methods in our Swift project.

To begin, we need to create a new Objective-C file to act as the bridging header.  Navigate to File -> New File

![](http://i.imgur.com/h1vkL8n.png)