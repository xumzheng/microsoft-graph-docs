---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Email = "AdeleV@contoso.com"
	ApplyHoldToSources = "true"
}

New-MgBetaComplianceEdiscoveryCaseCustodian -CaseId $caseId -BodyParameter $params

```