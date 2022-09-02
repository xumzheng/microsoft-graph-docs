---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CertificateBasedAuthConfigurationPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"certificateAuthorities" , new List<>
			{
				new 
				{
					IsRootAuthority = true,
					Certificate = "Binary",
				},
			}
		},
	},
};
await graphClient.Organization["organization-id"].CertificateBasedAuthConfiguration.PostAsync(requestBody);


```