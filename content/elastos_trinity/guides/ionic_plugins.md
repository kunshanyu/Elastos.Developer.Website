+++
title = "Ionic plugins"
weight = 20
chapter = false
pre = ""
alwaysopen = false
+++

## Ionic native apps vs Trinity apps

If you are familiar with ionic or cordova development, you already know that cordova native plugins can be added to your app according to your needs. For example, if you want to access device camera, this can't be done in pure Javascript code, and requires some native android/ios bridges through a cordova plugin.

In Trinity, the native Trinity application itself already embeds a **fixed set of plugins**. This means that **you cannot add your own native plugins**. 

Writing DApps for Trinity is different than writing ionic applications in the sense that Trinity DApps only deal with HTML/Javascript parts, and not with native parts (whereas native ionic apps mix both javascript and native code through plugins).

When you write a Trinity DApp, you can then access a **limited set of plugins** (you can find them in the Trinity plugins API reference), and nothing else.

## Application compilation

An other consequence of dealing only with javascript code in trinity is that **writing and releasing DApps don't require any compilation**, contrary to real ionic applications. You simply write your HTML/Javascript code, and send it to the trinity native app who will handle your DApp (using trinity-cli during development, or through the DApp store for distribution).
