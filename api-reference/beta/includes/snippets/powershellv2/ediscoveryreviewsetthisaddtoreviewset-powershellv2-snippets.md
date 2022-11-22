---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	Search = @{
		Id = "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7"
	}
	AdditionalDataOptions = "linkedFiles"
}

Add-MgBetaSecurityCaseEdiscoveryCaseReviewSetToReviewSet -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -BodyParameter $params

```