---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph..ExternalConnectors.Identity
{
	Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
	Type = IdentityType.User,
};
var result = await graphClient.External.Connections["externalConnection-id"].Groups["externalGroup-id"].Members.PostAsync(requestBody);


```