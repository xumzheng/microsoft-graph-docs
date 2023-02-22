---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userId = "55ac777c-109e-4022-b58c-470c8fcb6892";

var type = "Group";

await graphClient.Directory.DeletedItems
	.GetUserOwnedObjects(userId,type)
	.Request()
	.PostAsync();

```