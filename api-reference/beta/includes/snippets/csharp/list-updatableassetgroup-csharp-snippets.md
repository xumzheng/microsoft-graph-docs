---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAssetGroup = await graphClient.Admin.Windows.Updates.UpdatableAssets
	.Request()
	.GetAsync();

```