---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityUserFlowAttribute
{
	Description = "Your new hobby",
};
await graphClient.Identity.UserFlowAttributes["identityUserFlowAttribute-id"].PatchAsync(requestBody);


```