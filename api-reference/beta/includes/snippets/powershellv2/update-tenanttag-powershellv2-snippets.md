---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.ManagedTenants

$params = @{
	DisplayName = "Onboarding"
	Description = "Tenants that we are currently onboarding"
}

Update-MgBetaTenantRelationshipManagedTenantTag -TenantTagId $tenantTagId -BodyParameter $params

```