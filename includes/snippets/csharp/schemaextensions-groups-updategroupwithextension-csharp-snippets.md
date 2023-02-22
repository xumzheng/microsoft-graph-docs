---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
	AdditionalData = new Dictionary<string, object>()
	{
		{"graphlearn_courses", "{\"courseId\":\"123\",\"courseName\":\"New Managers\",\"courseType\":\"Online\"}"}
	}
};

await graphClient.Groups["{group-id}"]
	.Request()
	.UpdateAsync(group);

```