---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MembersRequestBody
{
	AdditionalData = new()
	{
		{"@odata.type", "#Microsoft.Graph.Group"},
		{"description", "Self help community for golf"},
		{"displayName", "Golf Assist"},
		{"groupTypes", new List<String>
		{
			"Unified",
		}
		{"mailEnabled", true},
		{"mailNickname", "golfassist"},
		{"securityEnabled", false},
	}
};
await graphClient.AdministrativeUnits["administrativeUnit-id"].Members.PostAsync(requestBody);


```