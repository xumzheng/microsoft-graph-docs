---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SectionGroupsRequestBody
{
	AdditionalData = new()
	{
		{"displayName", "Section group name"},
	}
};
await graphClient.Me.Onenote.SectionGroups["sectionGroup-id"].SectionGroups.PostAsync(requestBody);


```