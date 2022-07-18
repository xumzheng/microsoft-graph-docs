---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ExternalGroup
{
	DisplayName = "Contoso Marketing",
	Description = "The product marketing team",
};
await graphClient.External.Connections["externalConnection-id"].Groups["externalGroup-id"].PatchAsync(requestBody);


```