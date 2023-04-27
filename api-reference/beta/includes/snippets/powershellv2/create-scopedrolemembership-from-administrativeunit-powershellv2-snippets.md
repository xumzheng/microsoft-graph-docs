---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	roleId = "roleId-value"
	roleMemberInfo = @{
		id = "id-value"
	}
}

New-MgBetaAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```