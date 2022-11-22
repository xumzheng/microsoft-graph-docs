---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.ManagedTenants

$params = @{
	DisplayName = "Support"
	Description = "Tenants that have purchased extended support"
}

New-MgBetaTenantRelationshipManagedTenantTag -BodyParameter $params

```