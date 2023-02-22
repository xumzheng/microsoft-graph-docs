---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatePolicy = await graphClient.Admin.Windows.Updates.UpdatePolicies["{windowsUpdates.updatePolicy-id}"]
	.Request()
	.GetAsync();

```