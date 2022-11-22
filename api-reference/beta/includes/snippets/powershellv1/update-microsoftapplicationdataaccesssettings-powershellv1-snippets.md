---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgOrganizationSettingMicrosoftApplicationDataAccess -OrganizationId $organizationId -BodyParameter $params

```