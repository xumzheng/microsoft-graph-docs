---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LanguageProficiency
{
	DisplayName = "Norwegian Bokmål",
	Tag = "nb-NO",
	Spoken = LanguageProficiencyLevel.Nativeorbilingual,
	Written = LanguageProficiencyLevel.Nativeorbilingual,
	Reading = LanguageProficiencyLevel.Nativeorbilingual,
};
var result = await graphClient.Me.Profile.Languages.PostAsync(requestBody);


```