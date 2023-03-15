---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	IsEnabledInOrganization = $true
}

Update-MgBetaOrganizationSettingPronoun -OrganizationId $organizationId -BodyParameter $params

```