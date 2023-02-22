---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedUseServicePlans = await graphClient.DeviceManagement.VirtualEndpoint.SharedUseServicePlans
	.Request()
	.GetAsync();

```