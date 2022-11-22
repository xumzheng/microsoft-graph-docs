---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	ApplyHoldToSources = "false"
}

Update-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```