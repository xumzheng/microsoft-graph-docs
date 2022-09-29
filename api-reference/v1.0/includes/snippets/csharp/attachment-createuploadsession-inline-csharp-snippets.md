---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Me.Messages.Item.Attachments.CreateUploadSession.CreateUploadSessionPostRequestBody
{
	AttachmentItem = new AttachmentItem
	{
		AttachmentType = AttachmentType.File,
		Name = "scenary",
		Size = 7208534L,
		IsInline = true,
		ContentId = "my_inline_picture",
	},
};
var result = await graphClient.Me.Messages["message-id"].Attachments.CreateUploadSession.PostAsync(requestBody);


```