---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentApproval = await graphClient.Admin.Windows.Updates.UpdatePolicies["{windowsUpdates.updatePolicy-id}"].ComplianceChanges
	.Request()
	.GetAsync();

```