---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	Email = "AdeleV@contoso.com"
	ApplyHoldToSources = "true"
}

New-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -BodyParameter $params

```