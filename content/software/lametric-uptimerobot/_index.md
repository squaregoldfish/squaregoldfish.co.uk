---
title: 'UptimeRobot for LaMetric Time'
date: 2020-05-03:12:14+02:00
weight: 1
menu_page: true
---

Uptime Robot status for your LaMetric Time

<!--more-->
![UptimeRobot app running on LaMetric Time](/images/uptimerobot_lametric.jpg)

## Introduction
This is a simple app that displays the number of Up, Down, and (optionally) Paused
monitors from your [Uptime Robot](https://www.uptimerobot.com) account on your
[LaMetric Time](https://lametric.com/en-US/time/overview). Hopefully it will
mostly display "ALL ⬆" because all your systems are running smoothly.

## Installation
Simply search for "Uptime Robot" in the LaMetric app store, and install it as
you would any other app.

## Options

### UptimeRobot API Account Key
This must be the Read-Only API Key for your Uptime Robot account, and is
required for the app to retrieve the details of your monitors.

To find your key, log in to Uptime Robot and go to the My Settings page. At the
bottom right of the page there is a section titles "API Settings":

![UptimeRobot API key settings](/images/uptimerobot_apikey.png)

Show the Read-Only API key (you can generate it if you don't already have one)
and copy it in to the field.

### Ignore Paused Monitors
If this is selected, Paused monitors are not shown, and the "All ⬆" status will
show even if you have Paused monitors.

## Disclaimer
This app is in no way affiliated with Uptime Robot.

## Privacy Policy
This app does not collect any personal information. Uptime Robot API keys are
not logged at any point - they are used to retrieve monitor status and are then
discarded.
