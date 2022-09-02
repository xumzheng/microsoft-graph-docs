---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Me.Todo.Lists.Item.Tasks.Item.Attachments.CreateUploadSession.CreateUploadSessionPostRequestBody
{
	AttachmentInfo = new AttachmentInfo
	{
		AttachmentType = AttachmentType.File,
		Name = "flower",
		Size = 3483322L,
	},
};
var result = await graphClient.Me.Todo.Lists["todoTaskList-id"].Tasks["todoTask-id"].Attachments.CreateUploadSession.PostAsync(requestBody);


```