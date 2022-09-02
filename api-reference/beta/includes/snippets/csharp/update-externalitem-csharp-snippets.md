---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.ExternalConnectors.ExternalItem
{
	Acl = new List<Microsoft.Graph.Beta.Models.ExternalConnectors.Acl>
	{
		new Acl
		{
			Type = Microsoft.Graph.Beta.Models.ExternalConnectors.AclType.Everyone,
			Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
			AccessType = Microsoft.Graph.Beta.Models.ExternalConnectors.AccessType.Grant,
		},
	},
};
await graphClient.External.Connections["externalConnection-id"].Items["externalItem-id"].PatchAsync(requestBody);


```