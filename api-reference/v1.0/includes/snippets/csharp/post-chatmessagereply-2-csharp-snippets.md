---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	CreatedDateTime = DateTimeOffset.Parse("2019-02-04T19:58:15.511Z"),
	From = new From
	{
		User = new Identity
		{
			Id = "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
			DisplayName = "John Doe",
		},
	},
	Body = new ItemBody
	{
		ContentType = BodyType.Html,
		Content = "Hello World",
	},
};
var result = await graphClient.Teams["team-id"].Channels["channel-id"].Messages["chatMessage-id"].Replies.PostAsync(requestBody);


```