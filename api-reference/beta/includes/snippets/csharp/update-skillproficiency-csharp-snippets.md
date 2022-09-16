---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SkillProficiency
{
	Categories = new List<string>
	{
		"Professional",
	},
	Proficiency = SkillProficiencyLevel.AdvancedProfessional,
};
await graphClient.Me.Profile.Skills["skillProficiency-id"].PatchAsync(requestBody);


```