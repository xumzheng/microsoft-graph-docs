---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Site = @{
		WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
	}
}

New-MgBetaComplianceEdiscoveryCaseLegalHoldSiteSource -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```