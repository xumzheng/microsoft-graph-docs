---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OutlookCategory
{
	Color = CategoryColor.Preset15,
};
await graphClient.Me.Outlook.MasterCategories["outlookCategory-id"].PatchAsync(requestBody);


```