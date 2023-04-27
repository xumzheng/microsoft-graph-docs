---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	applyHoldToSource = $false
	dataSource = @{
		"@odata.type" = "microsoft.graph.ediscovery.siteSource"
	}
}

New-MgBetaComplianceEdiscoveryCaseNoncustodialDataSource -CaseId $caseId -BodyParameter $params

```