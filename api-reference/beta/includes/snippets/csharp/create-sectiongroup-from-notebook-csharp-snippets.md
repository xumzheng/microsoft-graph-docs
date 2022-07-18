---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SectionGroup
{
	DisplayName = "Section group name",
};
var result = await graphClient.Me.Onenote.Notebooks["notebook-id"].SectionGroups.PostAsync(requestBody);


```