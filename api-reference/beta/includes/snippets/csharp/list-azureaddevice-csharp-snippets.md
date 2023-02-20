---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var azureADDevice = await graphClient.Admin.Windows.Updates.UpdatableAssets
	.Request()
	.GetAsync();

```