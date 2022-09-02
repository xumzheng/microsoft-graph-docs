---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Groups.Item.Threads.Item.Reply.ReplyPostRequestBody
{
	Post = new Post
	{
		Body = new ItemBody
		{
			ContentType = BodyType.Text,
			Content = "Which quarter does that file cover? See my attachment.",
		},
		Attachments = new List<Attachment>
		{
			new Attachment
			{
				OdataType = "#microsoft.graph.fileAttachment",
				Name = "Another file as attachment",
				AdditionalData = new Dictionary<string, object>
				{
					{
						"contentBytes" , "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
					},
				},
			},
		},
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Reply.PostAsync(requestBody);


```