---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dismissReason = "Application is no longer needed.";

await graphClient.Directory.Recommendations["{recommendation-id}"].ImpactedResources["{impactedResource-id}"]
	.Dismiss(dismissReason)
	.Request()
	.PostAsync();

```