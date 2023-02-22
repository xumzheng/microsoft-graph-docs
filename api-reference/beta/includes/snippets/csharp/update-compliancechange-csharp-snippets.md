---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var complianceChange = new Microsoft.Graph.WindowsUpdates.ComplianceChange
{
	IsRevoked = true
};

await graphClient.Admin.Windows.Updates.UpdatePolicies["{windowsUpdates.updatePolicy-id}"].ComplianceChanges["{windowsUpdates.complianceChange-id}"]
	.Request()
	.UpdateAsync(complianceChange);

```