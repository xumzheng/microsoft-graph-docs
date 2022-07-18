---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Message
{
	ReceivedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
	SentDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
	HasAttachments = true,
	Subject = "subject-value",
	Body = new ItemBody
	{
		ContentType = "",
		Content = "content-value",
	},
	BodyPreview = "bodyPreview-value",
};
var result = await graphClient.Me.MailFolders["mailFolder-id"].Messages.PostAsync(requestBody);


```