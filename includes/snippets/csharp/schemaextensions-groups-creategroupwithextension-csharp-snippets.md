---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
	DisplayName = "New Managers March 2017",
	Description = "New Managers training course for March 2017",
	GroupTypes = new List<String>()
	{
		"Unified"
	},
	MailEnabled = true,
	MailNickname = "newMan201703",
	SecurityEnabled = false,
	AdditionalData = new Dictionary<string, object>()
	{
		{"graphlearn_courses", "{\"courseId\":\"123\",\"courseName\":\"New Managers\",\"courseType\":\"Online\"}"}
	}
};

await graphClient.Groups
	.Request()
	.AddAsync(group);

```