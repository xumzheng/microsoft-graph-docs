---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchemaRequestBody
{
	AdditionalData = new()
	{
		{"baseType", "microsoft.graph.externalItem"},
		{"properties", new List<Object>
		{
		}
	}
};
await graphClient.External.Connections["externalConnection-id"].Schema.PostAsync(requestBody);


```