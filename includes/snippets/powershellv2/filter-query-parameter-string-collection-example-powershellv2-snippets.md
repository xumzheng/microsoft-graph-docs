---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "imAddresses/any(i:i eq 'admin@contoso.com')" 

```