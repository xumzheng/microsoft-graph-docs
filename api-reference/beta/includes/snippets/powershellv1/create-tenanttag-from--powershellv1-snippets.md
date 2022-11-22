---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.ManagedTenants

$params = @{
	DisplayName = "Support"
	Description = "Tenants that have purchased extended support"
}

New-MgTenantRelationshipManagedTenantTag -BodyParameter $params

```