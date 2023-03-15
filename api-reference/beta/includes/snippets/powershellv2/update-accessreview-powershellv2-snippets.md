---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "TestReview new name"
}

Update-MgBetaAccessReview -AccessReviewId $accessReviewId -BodyParameter $params

```