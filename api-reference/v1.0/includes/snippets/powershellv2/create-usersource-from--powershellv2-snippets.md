---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	email = "admin@M365x809305.onmicrosoft.com"
	includedSources = "mailbox, site"
}

New-MgSecurityCaseEdiscoveryCaseCustodianUserSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryCustodianId $ediscoveryCustodianId -BodyParameter $params

```