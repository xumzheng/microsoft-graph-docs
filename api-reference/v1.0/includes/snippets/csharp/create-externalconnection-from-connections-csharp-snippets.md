---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.ExternalConnectors.ExternalConnection
{
	Id = "contosohr",
	Name = "Contoso HR",
	Description = "Connection to index Contoso HR system",
};
var result = await graphClient.External.Connections.PostAsync(requestBody);


```