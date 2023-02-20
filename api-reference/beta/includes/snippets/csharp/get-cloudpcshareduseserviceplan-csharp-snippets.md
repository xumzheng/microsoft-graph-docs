---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcSharedUseServicePlan = await graphClient.DeviceManagement.VirtualEndpoint.SharedUseServicePlans["{cloudPcSharedUseServicePlan-id}"]
	.Request()
	.GetAsync();

```