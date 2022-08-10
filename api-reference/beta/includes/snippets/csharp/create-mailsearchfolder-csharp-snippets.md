---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MailFolder
{
	OdataType = "microsoft.graph.mailSearchFolder",
	DisplayName = "Weekly digests",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"includeNestedFolders" , true
		},
		{
			"sourceFolderIds" , new List<>
			{
				"AQMkADYAAAIBDAAAAA==",
			}
		},
		{
			"filterQuery" , "contains(subject, 'weekly digest')"
		},
	},
};
var result = await graphClient.Me.MailFolders["mailFolder-id"].ChildFolders.PostAsync(requestBody);


```