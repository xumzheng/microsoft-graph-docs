---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new User
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"ext55gb1l09_msLearnCourses" , new 
			{
				CourseType = "Admin",
			}
		},
	},
};
await graphClient.Users["user-id"].PatchAsync(requestBody);


```