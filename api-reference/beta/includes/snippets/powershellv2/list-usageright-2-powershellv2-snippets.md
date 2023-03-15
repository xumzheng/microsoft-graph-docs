---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaDeviceUsageRights -DeviceId $deviceId -Filter "state in ('active', 'suspended') and serviceIdentifier in ('ABCD')" 

```