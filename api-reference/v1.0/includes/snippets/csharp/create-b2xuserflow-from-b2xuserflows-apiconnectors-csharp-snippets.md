---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new B2xIdentityUserFlow
{
	Id = "UserFlowWithAPIConnector",
	UserFlowType = "signUpOrSignIn",
	UserFlowTypeVersion = 1f,
	ApiConnectorConfiguration = new UserFlowApiConnectorConfiguration
	{
		PostFederationSignup = new 
		{
			AdditionalData = new()
			{
				{"@odata.id", "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"},
			}
		},
		PostAttributeCollection = new 
		{
			AdditionalData = new()
			{
				{"@odata.id", "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"},
			}
		},
	},
};
var result = await graphClient.Identity.B2xUserFlows.PostAsync(requestBody);


```