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
	.Filter("customSecurityAttributes/Marketing/AppCountry eq 'Canada'")
	.Select("id,displayName,customSecurityAttributes")
	.GetAsync();

```