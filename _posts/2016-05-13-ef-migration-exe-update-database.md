---
layout: post
title: EF migration.exe 'update-database'
categories: EF Enitity Framework update database update-database
---
It is possible to use the migration.exe file to fire a update-database statement against your builded/compiled project. Launch it through powershell. Example command:


<!-- language: lang-none -->
    # These variables should be set via the Octopus web portal:
    #
    #   ConnectionString         - The .Net connection string for the DB


    Write-Host "Connection String: <"$ConnectionString">"

    # Get the exe name based on the directory
    $contentPath  = (Join-Path "C:\wwwroot\test.permissionservice" "bin")
    $fullPath = (Join-Path $contentPath "migrate.exe")
    Write-Host "Migrate Path:" $fullPath

    cd $contentPath
    write-host "Working Dir: "$(get-location)

    # Run the migration utility
    & ".\migrate.exe" Core.dll /startUpConfigurationFile="../Web.config" /connectionString="Server=server;User   Id=userId;Password=password;" /connectionProviderName="System.Data.SqlClient" /verbose | Write-Host
