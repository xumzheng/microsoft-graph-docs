---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "TestReview new name"
}

Update-MgAccessReview -AccessReviewId $accessReviewId -BodyParameter $params

```