---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PostRequestBody
{
	Post = new Post
	{
		Body = new ItemBody
		{
			ContentType = "",
			Content = "content-value",
		},
		ReceivedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
		HasAttachments = true,
		From = new Recipient
		{
			EmailAddress = new EmailAddress
			{
				Name = "name-value",
				Address = "address-value",
			},
		},
		Sender = new Recipient
		{
			EmailAddress = new EmailAddress
			{
				Name = "name-value",
				Address = "address-value",
			},
		},
		ConversationThreadId = "conversationThreadId-value",
		NewParticipants = new List<Recipient>
		{
			new Recipient
			{
				AdditionalData = new()
				{
				}
			},
		}
		ConversationId = "conversationId-value",
		CreatedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
		LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
		ChangeKey = "changeKey-value",
		Categories = new List<String>
		{
			"categories-value",
		}
		Id = "id-value",
		InReplyTo = new 
		{
		},
		Attachments = new List<Attachment>
		{
			new Attachment
			{
				@odata.type = "#microsoft.graph.fileAttachment",
				LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
				Name = "name-value",
				ContentType = "contentType-value",
				Size = 99,
				IsInline = true,
				Id = "id-value",
			},
		}
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Posts["post-id"].Reply.PostAsync(requestBody);


```