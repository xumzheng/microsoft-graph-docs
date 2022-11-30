---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	Email = "megan@contoso.com"
	IncludedSources = "mailbox, site"
}

New-MgComplianceEdiscoveryCaseCustodianUserSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```