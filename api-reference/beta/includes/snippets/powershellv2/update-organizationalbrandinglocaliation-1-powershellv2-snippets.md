---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	signInPageText = "Default"
	usernameHintText = "DefaultHint"
}

Update-MgBetaOrganizationBranding -OrganizationId $organizationId -BodyParameter $params

```