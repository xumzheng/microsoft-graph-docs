---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.ExternalConnectors.ExternalGroup
{
	Id = "31bea3d537902000",
	DisplayName = "Contoso Marketing",
	Description = "The product marketing team",
};
var result = await graphClient.External.Connections["externalConnection-id"].Groups.PostAsync(requestBody);


```