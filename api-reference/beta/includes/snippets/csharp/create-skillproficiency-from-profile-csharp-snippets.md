---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SkillProficiency
{
	Categories = new List<String>
	{
		"Professional",
	}
	AllowedAudiences = "organization",
	DisplayName = "API Design",
	Proficiency = "generalProfessional",
	CollaborationTags = new List<String>
	{
		"ableToMentor",
	}
};
var result = await graphClient.Me.Profile.Skills.PostAsync(requestBody);


```