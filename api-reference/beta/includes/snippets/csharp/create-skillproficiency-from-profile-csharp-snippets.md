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
	AllowedAudiences = AllowedAudiences.Organization,
	DisplayName = "API Design",
	Proficiency = SkillProficiencyLevel.Generalprofessional,
	CollaborationTags = new List<string>
	{
		"ableToMentor",
	},
};
var result = await graphClient.Me.Profile.Skills.PostAsync(requestBody);


```