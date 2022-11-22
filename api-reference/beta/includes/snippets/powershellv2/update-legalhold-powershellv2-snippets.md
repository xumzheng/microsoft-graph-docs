---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Description = "This is a description for a legalHold"
}

Update-MgBetaComplianceEdiscoveryCaseLegalHold -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```