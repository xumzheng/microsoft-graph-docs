---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	OdataType = "#Microsoft.OutlookServices.FileAttachment",
	Name = "name-value",
	ContentType = "contentType-value",
	IsInline = false,
	AdditionalData = new Dictionary<string, object>
	{
		{
			"contentLocation" , "contentLocation-value"
		},
		{
			"contentBytes" , "contentBytes-value"
		},
	},
};
var result = await graphClient.Me.Messages["message-id"].Attachments.PostAsync(requestBody);


```