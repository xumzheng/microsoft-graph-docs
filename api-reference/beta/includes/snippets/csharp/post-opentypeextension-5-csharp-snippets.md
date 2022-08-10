---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Conversation
{
	Topic = "Does anyone have a second?",
	Threads = new List<ConversationThread>
	{
		new ConversationThread
		{
			Posts = new List<Post>
			{
				new Post
				{
					Body = new ItemBody
					{
						ContentType = BodyType.Html,
						Content = "This is urgent!",
					},
					Extensions = new List<Extension>
					{
						new Extension
						{
							OdataType = "microsoft.graph.openTypeExtension",
							AdditionalData = new Dictionary<string, object>
							{
								{
									"extensionName" , "Com.Contoso.Benefits"
								},
								{
									"companyName" , "Contoso"
								},
								{
									"expirationDate" , "2016-08-03T11:00:00.000Z"
								},
								{
									"topPicks" , new List<>
									{
										"Employees only",
										"Add spouse or guest",
										"Add family",
									}
								},
							},
						},
					},
				},
			},
		},
	},
};
var result = await graphClient.Groups["group-id"].Conversations.PostAsync(requestBody);


```