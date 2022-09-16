---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MailFolder
{
	OdataType = "microsoft.graph.mailSearchFolder",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"filterQuery" , "contains(subject, 'Analytics')"
		},
	},
};
await graphClient.Me.MailFolders["mailFolder-id"].PatchAsync(requestBody);


```