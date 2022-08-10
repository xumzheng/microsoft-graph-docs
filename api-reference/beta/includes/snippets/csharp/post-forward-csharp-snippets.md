---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ForwardPostRequestBody
{
	Comment = "comment-value",
	ToRecipients = new List<Recipient>
	{
		new Recipient
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"emailAddress" , new 
					{
						Name = "name-value",
						Address = "address-value",
					}
				},
			},
		},
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Posts["post-id"].Forward.PostAsync(requestBody);


```