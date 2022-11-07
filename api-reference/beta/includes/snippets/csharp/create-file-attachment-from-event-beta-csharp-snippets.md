---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	OdataType = "#microsoft.graph.fileAttachment",
	Name = "menu.txt",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"contentBytes" , "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
		},
	},
};
var result = await graphClient.Me.Events["event-id"].Attachments.PostAsync(requestBody);


```