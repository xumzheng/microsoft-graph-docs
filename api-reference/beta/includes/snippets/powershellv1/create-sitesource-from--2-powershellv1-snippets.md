---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Compliance

$params = @{
	Site = @{
		WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
	}
}

New-MgComplianceEdiscoveryCaseLegalHoldSiteSource -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```