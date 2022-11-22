---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	Site = @{
		WebUrl = "https://contoso.sharepoint.com/sites/HumanResources"
	}
}

New-MgComplianceEdiscoveryCaseCustodianSiteSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```