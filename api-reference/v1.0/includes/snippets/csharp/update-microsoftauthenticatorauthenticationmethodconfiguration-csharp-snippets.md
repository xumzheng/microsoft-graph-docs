---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodConfiguration
{
	OdataType = "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
	State = AuthenticationMethodState.Enabled,
};
await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["authenticationMethodConfiguration-id"].PatchAsync(requestBody);


```