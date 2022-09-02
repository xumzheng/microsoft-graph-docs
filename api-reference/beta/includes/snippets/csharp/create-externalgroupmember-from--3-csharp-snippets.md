---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..ExternalConnectors.Identity
{
	Id = "1431b9c38ee647f6a",
	Type = IdentityType.Externalgroup,
};
var result = await graphClient.External.Connections["externalConnection-id"].Groups["externalGroup-id"].Members.PostAsync(requestBody);


```