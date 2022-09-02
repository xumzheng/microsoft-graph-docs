---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.ReferenceCreate
{
	OdataId = "https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2",
};
await graphClient.DirectoryRoles["directoryRole-id"].Members.Ref.PostAsync(requestBody);


```