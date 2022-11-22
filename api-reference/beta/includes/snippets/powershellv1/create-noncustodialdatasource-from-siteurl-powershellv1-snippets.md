---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	ApplyHoldToSource = $false
	DataSource = @{
		"@odata.type" = "microsoft.graph.ediscovery.siteSource"
	}
}

New-MgComplianceEdiscoveryCaseNoncustodialDataSource -CaseId $caseId -BodyParameter $params

```