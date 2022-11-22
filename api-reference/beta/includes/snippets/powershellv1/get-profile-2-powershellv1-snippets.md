---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfile -UserId $userId -ExpandProperty "names(`$select=first,last),skills(`$select=displayName)" 

```