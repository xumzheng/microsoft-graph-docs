---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	Email = "adelev@contoso.com"
	IncludedSources = "mailbox"
}

New-MgComplianceEdiscoveryCaseLegalHoldUserSource -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```