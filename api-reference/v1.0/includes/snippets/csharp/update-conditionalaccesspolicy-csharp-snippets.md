---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConditionalAccessPolicy
{
	Conditions = new ConditionalAccessConditionSet
	{
		SignInRiskLevels = new List<RiskLevel>
		{
			RiskLevel.High,
			RiskLevel.Medium,
			RiskLevel.Low,
		},
	},
};
await graphClient.Identity.ConditionalAccess.Policies["conditionalAccessPolicy-id"].PatchAsync(requestBody);


```