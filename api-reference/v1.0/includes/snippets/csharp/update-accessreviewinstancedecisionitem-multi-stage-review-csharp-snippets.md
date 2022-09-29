---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewInstanceDecisionItem
{
	Decision = "Approve",
	Justification = "This person is still on my team",
};
var result = await graphClient.IdentityGovernance.AccessReviews.Definitions["accessReviewScheduleDefinition-id"].Instances["accessReviewInstance-id"].Stages["accessReviewStage-id"].Decisions["accessReviewInstanceDecisionItem-id"].PatchAsync(requestBody);


```