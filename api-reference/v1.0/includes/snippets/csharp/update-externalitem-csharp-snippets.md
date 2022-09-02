---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph..ExternalConnectors.ExternalItem
{
	Acl = new List<Microsoft.Graph..ExternalConnectors.Acl>
	{
		new Acl
		{
			Type = AclType.Everyone,
			Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
			AccessType = AccessType.Grant,
		},
	},
};
await graphClient.External.Connections["externalConnection-id"].Items["externalItem-id"].PatchAsync(requestBody);


```