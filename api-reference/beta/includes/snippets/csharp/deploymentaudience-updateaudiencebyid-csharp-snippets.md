---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UpdateAudienceByIdPostRequestBody
{
	MemberEntityType = "String",
	AddMembers = new List<>
	{
		"String",
	},
	RemoveMembers = new List<>
	{
		"String",
	},
	AddExclusions = new List<>
	{
		"String",
	},
	RemoveExclusions = new List<>
	{
		"String",
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].Audience.UpdateAudienceById.PostAsync(requestBody);


```