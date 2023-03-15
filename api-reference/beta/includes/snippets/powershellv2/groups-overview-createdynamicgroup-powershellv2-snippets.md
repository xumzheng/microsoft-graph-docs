---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Description = "Marketing department folks"
	DisplayName = "Marketing department"
	GroupTypes = @(
		"Unified"
		"DynamicMembership"
	)
	MailEnabled = $true
	MailNickname = "marketing"
	SecurityEnabled = $false
	MembershipRule = "user.department -eq "Marketing""
	MembershipRuleProcessingState = "on"
}

New-MgBetaGroup -BodyParameter $params

```