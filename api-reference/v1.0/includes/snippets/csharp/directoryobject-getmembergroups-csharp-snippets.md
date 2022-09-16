---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.DirectoryObjects.Item.GetMemberGroups.GetMemberGroupsPostRequestBody
{
	SecurityEnabledOnly = false,
};
var result = await graphClient.DirectoryObjects["directoryObject-id"].GetMemberGroups.PostAsync(requestBody);


```