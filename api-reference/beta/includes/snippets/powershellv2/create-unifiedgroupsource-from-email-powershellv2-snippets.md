---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	group = @{
		mail = "SecretGroup@contoso.com"
	}
	includedSources = "mailbox, site"
}

New-MgBetaComplianceEdiscoveryCaseCustodianUnifiedGroupSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```