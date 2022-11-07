---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationStrengthPolicy
{
	OdataType = "#microsoft.graph.authenticationStrengthPolicy",
	DisplayName = "FIDO2 only",
	Description = "An auth strength allowing only FIDO2 security keys.",
};
var result = await graphClient.Policies.AuthenticationStrengthPolicies["authenticationStrengthPolicy-id"].PatchAsync(requestBody);


```