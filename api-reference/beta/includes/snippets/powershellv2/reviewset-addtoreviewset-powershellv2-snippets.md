---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	SourceCollection = @{
		Id = "1a9b4145d8f84e39bc45a7f68c5c5119"
	}
	AdditionalData = "linkedFiles"
}

Add-MgBetaComplianceEdiscoveryCaseReviewSetToReviewSet -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```