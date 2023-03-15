---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Group = @{
		Mail = "SecretGroup@contoso.com"
	}
	IncludedSources = "mailbox, site"
}

New-MgBetaComplianceEdiscoveryCaseCustodianUnifiedGroupSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```