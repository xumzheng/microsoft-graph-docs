---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodConfiguration
{
	OdataType = "#microsoft.graph.fido2AuthenticationMethodConfiguration",
	State = AuthenticationMethodState.Enabled,
	AdditionalData = new Dictionary<string, object>
	{
		{
			"isAttestationEnforced" , "true"
		},
	},
};
await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["authenticationMethodConfiguration-id"].PatchAsync(requestBody);


```