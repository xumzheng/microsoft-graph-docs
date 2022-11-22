---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "startswith(displayName,'Eric')" -Property "displayName,signInActivity" 

```