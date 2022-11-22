---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	"@odata.type" = "#microsoft.graph.windowsUpdates.operationalInsightsConnection"
	AzureSubscriptionId = "322ec614-e9c2-4cd5-a55c-5711fdecf02e"
	AzureResourceGroupName = "target-resource-group"
	WorkspaceName = "my-workspace"
}

New-MgBetaWindowsUpdatesResourceConnection -BodyParameter $params

```