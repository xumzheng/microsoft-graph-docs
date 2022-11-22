---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	OutputName = "Export reviewset query via API"
	Description = "Export for the Contoso investigation 2"
	ExportOptions = "originalFiles,fileInfo,tags"
	ExportStructure = "directory"
}

Export-MgBetaSecurityCasesEdiscoveryCasesReviewSetsQuery -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -EdiscoveryReviewSetQueryId $ediscoveryReviewSetQueryId -BodyParameter $params

```