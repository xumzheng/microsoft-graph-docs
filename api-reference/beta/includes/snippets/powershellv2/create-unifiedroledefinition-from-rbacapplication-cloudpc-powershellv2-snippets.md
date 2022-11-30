---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Enrollment

$params = @{
	Description = "An example custom role"
	DisplayName = "ExampleCustomRole"
	RolePermissions = @(
		@{
			AllowedResourceActions = @(
				"Microsoft.CloudPC/CloudPCs/Read"
			)
		}
	)
	Condition = "null"
}

New-MgBetaRoleManagementCloudPcRoleDefinition -BodyParameter $params

```