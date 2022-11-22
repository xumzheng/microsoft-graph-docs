---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	DisplayName = "My Case 1 - Renamed"
	Description = "Updated description"
}

Update-MgBetaSecurityCaseEdiscoveryCase -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```