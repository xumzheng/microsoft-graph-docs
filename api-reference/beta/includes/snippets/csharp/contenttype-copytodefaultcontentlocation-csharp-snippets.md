---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CopyToDefaultContentLocationPostRequestBody
{
	SourceFile = new ItemReference
	{
		SharepointIds = new SharepointIds
		{
			ListId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
			ListItemId = "2",
		},
	},
	DestinationFileName = "newname.txt",
};
await graphClient.Sites["site-id"].ContentTypes["contentType-id"].CopyToDefaultContentLocation.PostAsync(requestBody);


```