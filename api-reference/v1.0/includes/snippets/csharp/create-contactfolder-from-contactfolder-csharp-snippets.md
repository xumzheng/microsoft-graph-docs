---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ContactFolder
{
	DisplayName = "Family",
};
var result = await graphClient.Me.ContactFolders["contactFolder-id"].ChildFolders.PostAsync(requestBody);


```