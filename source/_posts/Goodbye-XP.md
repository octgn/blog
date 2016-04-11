---
title: Goodbye XP
date: 2016-04-11 15:41:35
tags:
---

As of version 3.1.253.0 we are dropping support for Windows XP. At this time we will be supporting only Windows 7 or higher.

There are a few reasons we're doing this.

### MyGet
This is the main driving force behind our decisison. As of the beginning of March 2016(roughly) MyGet(or more correctly their CDN) dropped support for any SSL crypto algorithm that Windows XP has. Not specifically to block Windows XP, but because every crypto algorithm build into Windows XP is insecure. Because of this, users were unable to download games from MyGet, which effectively made OCTGN impossible to use anyways.

Now we though about it for awhile. We could have found another provider, or hosted our own NuGet feed, but it didn't seem to make sense, espeically due to the fact the Windows XP is not secure and not supported by even its creators.

### .NET Framework
OCTGN used the .NET Framework 4.0 it's whole life thus far. .NET Framework is supported on everything from Windows XP and up. The problem is that we miss out on lots of new technology, as the current .NET Framework version is 4.6.1. Also, .NET Framework 4.0 and 4.5 are end of life, so they are no longer being updated for security issues. This forces us to have to choose a higher version. We're going to choose .NET 4.6.1 going forward. Unfortunately Windows Vista doesn't support this version of the .NET Framework, so it has to be excluded as well.

### Support
We have a very small amount of people that do support, and no one is full time. A lot of bugs we end up getting are caused by users using outaded software(Windows XP). Removing the ability to use Windows XP will cause users to have a lot less issues with our software, and we will have a lot less wild bugs to squash.

### Wrap Up
So to summarize here, the main reason we're dropping support is because of security.

Thanks for reading, and have fun!
Kelly Elton
