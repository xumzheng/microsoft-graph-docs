---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dismissReason = "Recommendations is not relevant for my organization because...";

await graphClient.Directory.Recommendations["{recommendation-id}"]
	.Dismiss(dismissReason)
	.Request()
	.PostAsync();

```