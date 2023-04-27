---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	description = "Marketing group"
	displayName = "Marketing resources"
	mailEnabled = $false
	mailNickname = "markres"
	securityEnabled = $true
}

New-MgGroup -BodyParameter $params

```