---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new B2xIdentityUserFlow
{
	Id = "UserFlowWithAPIConnector",
	UserFlowType = UserFlowType.Signuporsignin,
	UserFlowTypeVersion = 1f,
	ApiConnectorConfiguration = new UserFlowApiConnectorConfiguration
	{
		PostFederationSignup = new PostFederationSignup
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.id" , "{apiConnectorId}"
				},
			},
		},
		PostAttributeCollection = new PostAttributeCollection
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.id" , "{apiConnectorId}"
				},
			},
		},
	},
};
var result = await graphClient.Identity.B2xUserFlows.PostAsync(requestBody);


```