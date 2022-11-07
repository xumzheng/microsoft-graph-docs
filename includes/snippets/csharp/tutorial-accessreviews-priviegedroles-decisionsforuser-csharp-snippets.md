---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.IdentityGovernance.AccessReviews.Definitions.Item.Instances.Item.Decisions.Item.Decision
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"decision" , "Deny"
		},
		{
			"justification" , "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'"
		},
	},
};
await graphClient.IdentityGovernance.AccessReviews.Definitions["accessReviewScheduleDefinition-id"].Instances["accessReviewInstance-id"].Decisions["accessReviewInstanceDecisionItem-id"].PostAsync(requestBody);


```