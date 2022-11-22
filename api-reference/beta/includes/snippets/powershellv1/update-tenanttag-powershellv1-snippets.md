---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.ManagedTenants

$params = @{
	DisplayName = "Onboarding"
	Description = "Tenants that we are currently onboarding"
}

Update-MgTenantRelationshipManagedTenantTag -TenantTagId $tenantTagId -BodyParameter $params

```