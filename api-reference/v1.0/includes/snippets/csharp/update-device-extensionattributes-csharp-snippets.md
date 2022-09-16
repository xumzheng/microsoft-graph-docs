---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Device
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"extensionAttributes" , new 
			{
				ExtensionAttribute1 = "BYOD-Device",
			}
		},
	},
};
await graphClient.Devices["device-id"].PatchAsync(requestBody);


```