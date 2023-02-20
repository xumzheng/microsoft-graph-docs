---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var postponeUntilDateTime = DateTimeOffset.Parse("2023-02-01T02:53:00Z");

await graphClient.Directory.Recommendations["{recommendation-id}"]
	.Postpone(postponeUntilDateTime)
	.Request()
	.PostAsync();

```