---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Me.Onenote.Notebooks.Item.CopyNotebook.CopyNotebookPostRequestBody
{
	GroupId = "groupId-value",
	RenameAs = "renameAs-value",
};
var result = await graphClient.Me.Onenote.Notebooks["notebook-id"].CopyNotebook.PostAsync(requestBody);


```