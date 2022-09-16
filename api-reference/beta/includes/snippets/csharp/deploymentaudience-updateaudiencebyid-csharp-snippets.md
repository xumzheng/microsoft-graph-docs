---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Admin.Windows.Updates.Deployments.Item.Audience.UpdateAudienceById.UpdateAudienceByIdPostRequestBody
{
	MemberEntityType = "String",
	AddMembers = new List<string>
	{
		"String",
	},
	RemoveMembers = new List<string>
	{
		"String",
	},
	AddExclusions = new List<string>
	{
		"String",
	},
	RemoveExclusions = new List<string>
	{
		"String",
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].Audience.UpdateAudienceById.PostAsync(requestBody);


```