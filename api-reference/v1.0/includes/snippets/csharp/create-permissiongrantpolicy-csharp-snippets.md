---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PermissionGrantPolicy
{
	Id = "my-custom-consent-policy",
	DisplayName = "Custom application consent policy",
	Description = "A custom permission grant policy to customize conditions for granting consent.",
};
var result = await graphClient.Policies.PermissionGrantPolicies.PostAsync(requestBody);


```