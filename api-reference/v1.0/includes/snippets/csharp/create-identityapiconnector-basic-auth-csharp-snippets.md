---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityApiConnector
{
	DisplayName = "Test API",
	TargetUrl = "https://someapi.com/api",
	AuthenticationConfiguration = new ApiAuthenticationConfigurationBase
	{
		OdataType = "#microsoft.graph.basicAuthentication",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"username" , "MyUsername"
			},
			{
				"password" , "MyPassword"
			},
		},
	},
};
var result = await graphClient.Identity.ApiConnectors.PostAsync(requestBody);


```