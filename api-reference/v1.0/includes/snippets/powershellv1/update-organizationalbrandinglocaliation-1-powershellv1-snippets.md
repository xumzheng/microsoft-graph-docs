---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	SignInPageText = "Default"
	UsernameHintText = "DefaultHint"
}

Update-MgOrganizationBranding -OrganizationId $organizationId -BodyParameter $params

```