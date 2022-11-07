---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationCombinationConfiguration
{
	AppliesToCombinations = new List<AuthenticationMethodModes?>
	{
		AuthenticationMethodModes.Fido2,
	},
};
var result = await graphClient.Identity.ConditionalAccess.AuthenticationStrengths.Policies["authenticationStrengthPolicy-id"].CombinationConfigurations["authenticationCombinationConfiguration-id"].PatchAsync(requestBody);


```