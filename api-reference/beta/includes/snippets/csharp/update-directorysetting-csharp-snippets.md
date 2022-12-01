---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DirectorySetting
{
	Values = new List<SettingValue>
	{
		new SettingValue
		{
			Name = "CustomBlockedWordsList",
			Value = "Contoso",
		},
	},
};
var result = await graphClient.Settings["directorySetting-id"].PatchAsync(requestBody);


```