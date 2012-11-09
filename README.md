MultitaskingBarNotifier
=======================

Notifications for when the iOS multitasking bar is showing.

This will be a cocoa implementation providing applications a notification when 
the iOS multitasking bar is shown or hidden. It is mainly for enabling custom
views when the task bar is shown (especially for instructions on how to enable
airplay/mirroring since there is no API to do this within 3rd party apps, at
least as of iOS 6).

A working implementation can be seen in the iPad version of Tip of the Tongue 
word game (developed by Owen Imholte) on the App Store. There is nothing to
prevent the method from working on iPhone, as well.

This repo is for the purpose of sharing and improving the (necessarily slightly
hackish) quality of the code.

I'll post the code as soon as possible, but for the interested the way it works
is by exploiting the applicationWillResignActive and applicationWillTerminate
notifications when showing the task bar vs. killing the app.