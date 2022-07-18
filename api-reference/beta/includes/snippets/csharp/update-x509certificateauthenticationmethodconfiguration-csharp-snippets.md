---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodConfiguration
{
	@odata.type = "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
	Id = "X509Certificate",
	State = "enabled",
	AdditionalData = new()
	{
		{"certificateUserBindings", new List<Object>
		{
		}
		{"includeTargets", new List<Object>
		{
		}
	}
};
await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["authenticationMethodConfiguration-id"].PatchAsync(requestBody);


```