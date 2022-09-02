---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Me.MailFolders.Item.Move.MovePostRequestBody
{
	DestinationId = "destinationId-value",
};
var result = await graphClient.Me.MailFolders["mailFolder-id"].Move.PostAsync(requestBody);


```