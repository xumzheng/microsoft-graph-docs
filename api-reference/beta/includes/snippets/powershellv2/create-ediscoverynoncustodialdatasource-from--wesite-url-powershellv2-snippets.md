---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	dataSource = @{
		"@odata.type" = "microsoft.graph.security.siteSource"
	}
}

New-MgBetaSecurityCaseEdiscoveryCaseNoncustodialDataSource -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```