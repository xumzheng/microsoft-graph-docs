---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	DisplayName = "My Case 1 - Renamed"
	Description = "Updated description"
	ExternalId = "Updated externalId"
}

Update-MgComplianceEdiscoveryCase -CaseId $caseId -BodyParameter $params

```