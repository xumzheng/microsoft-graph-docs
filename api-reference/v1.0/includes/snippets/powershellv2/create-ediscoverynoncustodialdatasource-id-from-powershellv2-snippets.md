---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	dataSource = @{
		"@odata.type" = "microsoft.graph.security.siteSource"
	}
}

New-MgSecurityCaseEdiscoveryCaseNoncustodialDataSource -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```