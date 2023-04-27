---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	backgroundColor = "#00000F"
	signInPageText = "Welcome to Contoso France"
}

Update-MgBetaOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId -BodyParameter $params

```