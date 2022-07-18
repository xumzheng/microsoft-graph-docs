---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	@odata.type = "#microsoft.graph.fileAttachment",
	Name = "menu.txt",
	AdditionalData = new()
	{
		{"contentBytes", "bWFjIGFuZCBjaGVlc2UgdG9kYXk="},
	}
};
var result = await graphClient.Me.Outlook.Tasks["outlookTask-id"].Attachments.PostAsync(requestBody);


```