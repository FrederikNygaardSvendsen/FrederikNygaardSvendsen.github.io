---
layout: post
title: c# misleading exception
categories: c# view full exception
---
In c#, if you get the stacktrace property of an exception, you will only get the outermost exception. If the cause is shown in an innser exception, this is not shown. You can full the full stacktrace, including all inner exceptions, by invoking tostring() on the exception itself.
