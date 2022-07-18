---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AddMembersByIdRequestBody
{
	Ids = new List<String>
	{
		"String",
		"String",
		"String",
	}
	MemberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice",
};
await graphClient.Admin.Windows.Updates.UpdatableAssets["updatableAsset-id"].AddMembersById.PostAsync(requestBody);


```