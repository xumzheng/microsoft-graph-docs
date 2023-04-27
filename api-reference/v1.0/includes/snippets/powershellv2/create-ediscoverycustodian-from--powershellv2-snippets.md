---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	email = "AdeleV@contoso.com"
}

New-MgSecurityCaseEdiscoveryCaseCustodian -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```