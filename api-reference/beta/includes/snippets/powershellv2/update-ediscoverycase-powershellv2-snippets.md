---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	displayName = "My Case 1 - Renamed"
	description = "Updated description"
}

Update-MgBetaSecurityCaseEdiscoveryCase -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```