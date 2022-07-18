---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewInstanceDecisionItem
{
	Decision = "Approve",
	Justification = "Kathleen still needs access to the Marketing group as she works in the Marketing organization.",
};
await graphClient.IdentityGovernance.AccessReviews.Definitions["accessReviewScheduleDefinition-id"].Instances["accessReviewInstance-id"].Decisions["accessReviewInstanceDecisionItem-id"].PatchAsync(requestBody);


```