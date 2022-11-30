---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	DisplayName = "My Reviewset 3"
}

New-MgBetaComplianceEdiscoveryCaseReviewSet -CaseId $caseId -BodyParameter $params

```