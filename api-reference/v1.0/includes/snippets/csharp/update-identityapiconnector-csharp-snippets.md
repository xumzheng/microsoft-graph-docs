---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityApiConnector
{
	AuthenticationConfiguration = new ApiAuthenticationConfigurationBase
	{
		@odata.type = "#microsoft.graph.pkcs12Certificate",
		AdditionalData = new()
		{
			{"pkcs12Value", "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA"},
			{"password", "secret"},
		}
	},
};
await graphClient.Identity.ApiConnectors["identityApiConnector-id"].PatchAsync(requestBody);


```