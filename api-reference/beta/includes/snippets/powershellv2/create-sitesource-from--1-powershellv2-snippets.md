---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Site = @{
		WebUrl = "https://contoso.sharepoint.com/sites/HumanResources"
	}
}

New-MgBetaComplianceEdiscoveryCaseCustodianSiteSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```