---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	description = "Marketing department folks"
	displayName = "Marketing department"
	groupTypes = @(
		"Unified"
		"DynamicMembership"
	)
	mailEnabled = $true
	mailNickname = "marketing"
	securityEnabled = $false
	membershipRule = "user.department -eq "Marketing""
	membershipRuleProcessingState = "on"
}

New-MgGroup -BodyParameter $params

```