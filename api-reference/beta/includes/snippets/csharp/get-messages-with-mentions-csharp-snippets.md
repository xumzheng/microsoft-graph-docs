---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Messages.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "MentionsPreview/IsMentioned%20eq%20true";
	requestConfiguration.QueryParameters.Select = new [] { "Subject" , "Sender" , "ReceivedDateTime" , "MentionsPreview" };
});


```