---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	displayName = "My Query 1 - Renamed"
}

Update-MgBetaComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -ReviewSetQueryId $reviewSetQueryId -BodyParameter $params

```