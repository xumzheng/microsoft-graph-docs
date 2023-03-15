---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	Group = @{
		Mail = "SOCTeam@M365x809305.onmicrosoft.com"
	}
	IncludedSources = "mailbox, site"
}

New-MgBetaSecurityCaseEdiscoveryCaseCustodianUnifiedGroupSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryCustodianId $ediscoveryCustodianId -BodyParameter $params

```