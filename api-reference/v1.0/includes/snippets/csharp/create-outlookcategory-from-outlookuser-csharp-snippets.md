---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OutlookCategory
{
	DisplayName = "Project expenses",
	Color = CategoryColor.Preset9,
};
var result = await graphClient.Me.Outlook.MasterCategories.PostAsync(requestBody);


```