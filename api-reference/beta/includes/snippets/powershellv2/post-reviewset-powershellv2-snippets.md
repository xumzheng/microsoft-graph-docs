---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	displayName = "My Reviewset 3"
}

New-MgBetaComplianceEdiscoveryCaseReviewSet -CaseId $caseId -BodyParameter $params

```