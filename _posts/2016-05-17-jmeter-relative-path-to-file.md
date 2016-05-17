---
layout: post
title: JMeter, relative path to file
categories: JMeter relative path file
---
To give the path to a file, relative to the .jmx file, use the following command:

<!-- language: lang-none -->
    ${__BeanShell(import org.apache.jmeter.services.FileServer; FileServer.getFileServer().getBaseDir();)}${__BeanShell(File.separator,)}<YOUR FILENAME HERE>

<!-- end the list -->
Ex.

<!-- language: lang-none -->
    ${__BeanShell(import org.apache.jmeter.services.FileServer; FileServer.getFileServer().getBaseDir();)}${__BeanShell(File.separator,)}MyFile.txt

<!-- end the list -->
