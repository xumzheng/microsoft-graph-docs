---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Messages.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "MentionsPreview/IsMentioned eq true";
	requestConfiguration.QueryParameters.Select = new string []{ "Subject","Sender","ReceivedDateTime","MentionsPreview" };
});


```