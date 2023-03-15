---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	IsEnabledInOrganization = $true
	DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgBetaOrganizationSettingPersonInsight -OrganizationId $organizationId -BodyParameter $params

```