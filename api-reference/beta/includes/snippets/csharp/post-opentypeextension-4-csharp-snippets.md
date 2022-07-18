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
			ContentType = "html",
			Content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>",
		},
		Extensions = new List<Extension>
		{
			new Extension
			{
				@odata.type = "microsoft.graph.openTypeExtension",
				AdditionalData = new()
				{
					{"extensionName", "Com.Contoso.HR"},
					{"companyName", "Contoso"},
					{"expirationDate", "2015-07-03T13:04:00.000Z"},
					{"topPicks", new List<String>
					{
						"Employees only",
						"Add spouse or guest",
						"Add family",
					}
				}
			},
		}
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Posts["post-id"].Reply.PostAsync(requestBody);


```