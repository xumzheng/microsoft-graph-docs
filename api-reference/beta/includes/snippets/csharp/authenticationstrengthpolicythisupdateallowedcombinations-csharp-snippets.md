---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Policies.AuthenticationStrengthPolicies.Item.UpdateAllowedCombinations.UpdateAllowedCombinationsPostRequestBody
{
	AllowedCombinations = new List<AuthenticationMethodModes?>
	{
		AuthenticationMethodModes.Password | AuthenticationMethodModes.Voice,
	},
};
var result = await graphClient.Policies.AuthenticationStrengthPolicies["authenticationStrengthPolicy-id"].UpdateAllowedCombinations.PostAsync(requestBody);


```