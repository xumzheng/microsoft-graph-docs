---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceCreate
{
	OdataId = "https://graph.microsoft.com/beta/users/alexd@contoso.com",
};
await graphClient.Groups["group-id"].AcceptedSenders.Ref.PostAsync(requestBody);


```