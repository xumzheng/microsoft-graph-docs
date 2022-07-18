---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	@odata.type = "microsoft.graph.fileAttachment",
	Name = "name-value",
	ContentType = "contentType-value",
	IsInline = false,
	AdditionalData = new()
	{
		{"contentLocation", "contentLocation-value"},
		{"contentBytes", "base64-contentBytes-value"},
	}
};
var result = await graphClient.Me.Messages["message-id"].Attachments.PostAsync(requestBody);


```