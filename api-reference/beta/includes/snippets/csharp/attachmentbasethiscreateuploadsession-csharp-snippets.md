---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AttachmentInfoRequestBody
{
	AttachmentInfo = new AttachmentInfo
	{
		AttachmentType = "file",
		Name = "flower",
		Size = 3483322L,
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.attachmentInfo"},
		}
	},
};
var result = await graphClient.Me.Todo.Lists["todoTaskList-id"].Tasks["todoTask-id"].Attachments.CreateUploadSession.PostAsync(requestBody);


```