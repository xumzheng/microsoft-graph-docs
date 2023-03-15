---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	DisplayName = "Seattle District Technical Schools"
	Description = "Seattle district technical schools administration"
	MembershipType = "Dynamic"
	MembershipRule = "(user.country -eq "United States")"
	MembershipRuleProcessingState = "On"
}

New-MgBetaAdministrativeUnit -BodyParameter $params

```