---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
	.Request()
	.Filter("graphlearn_courses/courseId eq '123'")
	.Select("displayName,id,description,graphlearn_courses")
	.GetAsync();

```