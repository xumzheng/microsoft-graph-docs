---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.ManagedTenants

$params = @{
	displayName = "Support"
	description = "Tenants that have purchased extended support"
}

New-MgBetaTenantRelationshipManagedTenantTag -BodyParameter $params

```