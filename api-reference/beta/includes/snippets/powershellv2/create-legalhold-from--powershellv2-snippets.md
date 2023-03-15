---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	"@odata.type" = "#microsoft.graph.ediscovery.legalHold"
	Description = "String"
	CreatedBy = @{
		"@odata.type" = "microsoft.graph.identitySet"
	}
	IsEnabled = "Boolean"
	Status = "String"
	ContentQuery = "String"
	Errors = @(
		"String"
	)
	DisplayName = "String"
}

New-MgBetaComplianceEdiscoveryCaseLegalHold -CaseId $caseId -BodyParameter $params

```