---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	applyHoldToSources = "false"
}

Update-MgBetaComplianceEdiscoveryCaseCustodian -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```