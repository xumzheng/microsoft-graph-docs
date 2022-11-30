---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	OutputName = "Export via API"
	Description = "Export for the Contoso investigation"
	ExportOptions = "originalFiles,fileInfo,tags"
	ExportStructure = "directory"
}

Export-MgBetaSecurityCasesEdiscoveryCasesReviewSet -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -BodyParameter $params

```