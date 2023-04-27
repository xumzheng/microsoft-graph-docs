---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	signInPageText = "Welcome to Contoso France."
	usernameHintText = " "
}

Update-MgBetaOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId -BodyParameter $params

```