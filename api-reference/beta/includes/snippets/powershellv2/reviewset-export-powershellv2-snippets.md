---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	OutputName = "2020-12-06 Contoso investigation export"
	Description = "Export for the Contoso investigation"
	ExportOptions = "originalFiles,fileInfo,tags"
	ExportStructure = "directory"
}

Export-MgBetaComplianceEdiscoveryCasesReviewSet -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```