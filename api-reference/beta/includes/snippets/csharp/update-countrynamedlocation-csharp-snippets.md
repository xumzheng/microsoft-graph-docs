---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NamedLocation
{
	@odata.type = "#microsoft.graph.countryNamedLocation",
	DisplayName = "Updated named location without unknown countries and regions",
	AdditionalData = new()
	{
		{"countriesAndRegions", new List<String>
		{
			"CA",
			"IN",
		}
		{"includeUnknownCountriesAndRegions", false},
	}
};
await graphClient.Identity.ConditionalAccess.NamedLocations["namedLocation-id"].PatchAsync(requestBody);


```