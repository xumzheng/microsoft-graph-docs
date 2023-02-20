---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
	new QueryOption("$count", "true")
};

var users = await graphClient.Users
	.Request( queryOptions )
	.Header("ConsistencyLevel","eventual")
	.Filter("startsWith(customSecurityAttributes/Marketing/EmployeeId,'GS')")
	.Select("id,displayName,customSecurityAttributes")
	.GetAsync();

```