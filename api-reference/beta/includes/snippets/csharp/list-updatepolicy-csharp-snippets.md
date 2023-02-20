---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatePolicies = await graphClient.Admin.Windows.Updates.UpdatePolicies
	.Request()
	.GetAsync();

```