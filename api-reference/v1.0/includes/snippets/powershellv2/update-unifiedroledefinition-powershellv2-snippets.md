---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	description = "Update basic properties of application registrations"
	displayName = "Application Registration Support Administrator"
	rolePermissions = @(
		@{
			allowedResourceActions = @(
				"microsoft.directory/applications/basic/read"
			)
		}
	)
}

Update-MgRoleManagementDirectoryRoleDefinition -UnifiedRoleDefinitionId $unifiedRoleDefinitionId -BodyParameter $params

```