---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcProvisioningPolicy"
	DisplayName = "HR provisioning policy"
	Description = "Provisioning policy for India HR employees"
	OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
	ImageId = "Image ID value"
	ImageDisplayName = "Image Display Name value"
	ImageType = "custom"
	WindowsSettings = @{
		Language = "en-US"
	}
}

Update-MgBetaDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -BodyParameter $params

```