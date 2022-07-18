---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UpdateAudienceByIdRequestBody
{
	MemberEntityType = "String",
	AddMembers = new List<String>
	{
		"String",
	}
	RemoveMembers = new List<String>
	{
		"String",
	}
	AddExclusions = new List<String>
	{
		"String",
	}
	RemoveExclusions = new List<String>
	{
		"String",
	}
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].Audience.UpdateAudienceById.PostAsync(requestBody);


```