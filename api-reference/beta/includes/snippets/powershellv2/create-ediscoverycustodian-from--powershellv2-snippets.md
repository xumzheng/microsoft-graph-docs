---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	email = "AdeleV@contoso.com"
}

New-MgBetaSecurityCaseEdiscoveryCaseCustodian -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```