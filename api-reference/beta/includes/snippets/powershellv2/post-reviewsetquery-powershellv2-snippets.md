---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	DisplayName = "My Query 1"
	Query = "(subject:"Quarterly Financials")"
}

New-MgBetaComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```