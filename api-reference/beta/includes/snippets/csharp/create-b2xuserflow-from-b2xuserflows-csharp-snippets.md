---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new B2xIdentityUserFlow
{
	Id = "Partner",
	UserFlowType = UserFlowType.Signuporsignin,
	UserFlowTypeVersion = 1f,
};
var result = await graphClient.Identity.B2xUserFlows.PostAsync(requestBody);


```