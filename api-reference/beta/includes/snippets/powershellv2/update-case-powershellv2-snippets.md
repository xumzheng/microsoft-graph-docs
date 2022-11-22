---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	DisplayName = "My Case 1 - Renamed"
	Description = "Updated description"
	ExternalId = "Updated externalId"
}

Update-MgBetaComplianceEdiscoveryCase -CaseId $caseId -BodyParameter $params

```