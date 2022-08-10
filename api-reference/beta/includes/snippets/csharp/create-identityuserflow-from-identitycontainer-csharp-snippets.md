---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityUserFlow
{
	Id = "Pol1",
	UserFlowType = UserFlowType.Signuporsignin,
	UserFlowTypeVersion = 1f,
};
var result = await graphClient.Identity.UserFlows.PostAsync(requestBody);


```