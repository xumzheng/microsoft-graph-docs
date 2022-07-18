---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	@odata.type = "#microsoft.graph.fileAttachment",
	Name = "smile",
	AdditionalData = new()
	{
		{"contentBytes", "R0lGODdhEAYEAA7"},
	}
};
var result = await graphClient.Me.Messages["message-id"].Attachments.PostAsync(requestBody);


```