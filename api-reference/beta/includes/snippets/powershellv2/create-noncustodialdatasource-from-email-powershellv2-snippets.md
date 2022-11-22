---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	ApplyHoldToSource = $true
	DataSource = @{
		"@odata.type" = "microsoft.graph.ediscovery.userSource"
		Email = "adelev@contoso.com"
	}
}

New-MgBetaComplianceEdiscoveryCaseNoncustodialDataSource -CaseId $caseId -BodyParameter $params

```