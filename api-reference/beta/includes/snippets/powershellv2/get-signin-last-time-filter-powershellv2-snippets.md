---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

Get-MgBetaUser -Filter "startswith(displayName,'Eric')" -Property "displayName,signInActivity" 

```