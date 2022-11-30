---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Description = "Self help community for golf"
	DisplayName = "Golf Assist"
	GroupTypes = @(
		"Unified"
	)
	MailEnabled = $true
	MailNickname = "golfassist"
	SecurityEnabled = $false
}

New-MgBetaGroup -BodyParameter $params

```