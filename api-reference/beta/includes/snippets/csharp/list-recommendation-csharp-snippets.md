---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recommendations = await graphClient.Directory.Recommendations
	.Request()
	.GetAsync();

```