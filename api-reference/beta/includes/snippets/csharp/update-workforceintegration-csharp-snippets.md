---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new WorkforceIntegration
{
	DisplayName = "displayName-value",
	ApiVersion = 99,
	Encryption = new WorkforceIntegrationEncryption
	{
		Protocol = WorkforceIntegrationEncryptionProtocol.SharedSecret,
		Secret = "secret-value",
	},
	IsActive = true,
	Url = "url-value",
	Supports = WorkforceIntegrationSupportedEntities.None,
};
var result = await graphClient.Teamwork.WorkforceIntegrations["workforceIntegration-id"].PatchAsync(requestBody);


```