---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Admin.Windows.Updates.UpdatePolicies["{windowsUpdates.updatePolicy-id}"]
	.Request()
	.DeleteAsync();

```