---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NamedLocation
{
	@odata.type = "#microsoft.graph.ipNamedLocation",
	DisplayName = "Untrusted named location with only IPv4 address",
	AdditionalData = new()
	{
		{"isTrusted", false},
		{"ipRanges", new List<Object>
		{
		}
	}
};
await graphClient.Identity.ConditionalAccess.NamedLocations["namedLocation-id"].PatchAsync(requestBody);


```