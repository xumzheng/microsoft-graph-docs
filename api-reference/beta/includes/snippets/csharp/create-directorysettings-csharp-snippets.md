---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DirectorySetting
{
	TemplateId = "62375ab9-6b52-47ed-826b-58e47e0e304b",
	Values = new List<SettingValue>
	{
		new SettingValue
		{
			Name = "GuestUsageGuidelinesUrl",
			Value = "https://privacy.contoso.com/privacystatement",
		},
		new SettingValue
		{
			Name = "EnableMSStandardBlockedWords",
			Value = "true",
		},
		new SettingValue
		{
			Name = "EnableMIPLabels",
			Value = "true",
		},
		new SettingValue
		{
			Name = "PrefixSuffixNamingRequirement",
			Value = "[Contoso-][GroupName]",
		},
	},
};
var result = await graphClient.Settings.PostAsync(requestBody);


```