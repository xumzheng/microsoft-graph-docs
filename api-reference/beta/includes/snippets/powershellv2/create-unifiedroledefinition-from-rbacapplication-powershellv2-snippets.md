---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Description = "Update basic properties of application registrations"
	DisplayName = "Application Registration Support Administrator"
	RolePermissions = @(
		@{
			AllowedResourceActions = @(
				"microsoft.directory/applications/basic/read"
			)
		}
	)
	IsEnabled = "true"
}

New-MgBetaRoleManagementDirectoryRoleDefinition -BodyParameter $params

```