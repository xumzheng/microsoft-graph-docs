---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CustomSecurityAttributeDefinition
{
	AdditionalData = new()
	{
		{"allowedValues@delta", new List<Object>
		{
		}
	}
};
await graphClient.Directory.CustomSecurityAttributeDefinitions["customSecurityAttributeDefinition-id"].PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("OData-Version", "4.01");
});


```