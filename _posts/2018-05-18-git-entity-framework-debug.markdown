---
layout: post
title:  "Entity Framework errormessage debug"
date:   2018-05-18 14:34:34 +0100
categories: entity-framework
---
Try putting the SQL statements directly into the MySQL Workbench.

    1. Type "dotnet ef migrations script" in your commandprompt.
    2. Copy the generated SQL script.
    3. Paste it into your Workbench.
    4. Check where the errors occur.


When I got errors using EF core 2 with MySQL this helped me understand the problem better and helped solve the problem. (for me it was a typing error). You can at least use this method to determine if it is an error in the migrations or in your SQL statements.