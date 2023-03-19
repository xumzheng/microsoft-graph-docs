---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaDeviceMemberOf -DeviceId $deviceId -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "displayName" -Filter "startswith(displayName, 'A')" -ConsistencyLevel eventual 


```