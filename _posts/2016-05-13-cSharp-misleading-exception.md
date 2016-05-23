---
layout: post
title: c#, misleading exception stacktrace
tags:
- exception
- stacktrace
---
In c#, if you get the stacktrace property of an exception, you will only get the outermost exception. If the cause is shown in an inner exception, this is not shown. You can get the full stacktrace, including all inner exceptions, by invoking tostring() on the exception itself.
