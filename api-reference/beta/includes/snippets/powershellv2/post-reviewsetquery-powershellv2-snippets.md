---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	displayName = "My Query 1"
	query = "(subject:"Quarterly Financials")"
}

New-MgBetaComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```