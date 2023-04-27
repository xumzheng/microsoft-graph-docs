---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	displayName = "Quarterly Financials search"
}

Update-MgBetaComplianceEdiscoveryCaseSourceCollection -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```