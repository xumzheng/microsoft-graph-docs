---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcDeviceImage"
	DisplayName = "Display Name value"
	OsBuildNumber = "OS Build Number value"
	OperatingSystem = "Operating System value"
	Version = "Version value"
	SourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}

New-MgBetaDeviceManagementVirtualEndpointDeviceImage -BodyParameter $params

```