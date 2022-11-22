---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	DisplayName = "My Reviewset 3"
}

New-MgComplianceEdiscoveryCaseReviewSet -CaseId $caseId -BodyParameter $params

```