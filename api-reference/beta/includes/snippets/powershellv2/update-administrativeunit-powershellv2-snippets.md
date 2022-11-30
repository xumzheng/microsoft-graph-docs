---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	MembershipType = "Dynamic"
	MembershipRule = "(user.country -eq "United States")"
	MembershipRuleProcessingState = "On"
}

Update-MgBetaAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```