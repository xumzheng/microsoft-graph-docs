---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.ExternalConnectors.Identity
{
	Id = "1431b9c38ee647f6a",
	Type = Microsoft.Graph.Beta.Models.ExternalConnectors.IdentityType.ExternalGroup,
};
var result = await graphClient.External.Connections["externalConnection-id"].Groups["externalGroup-id"].Members.PostAsync(requestBody);


```