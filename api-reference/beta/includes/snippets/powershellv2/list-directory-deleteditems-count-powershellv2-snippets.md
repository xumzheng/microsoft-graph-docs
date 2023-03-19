---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaDirectoryDeletedItem -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "deletedDateTime asc" -Property "id,displayName,deletedDateTime" 

```