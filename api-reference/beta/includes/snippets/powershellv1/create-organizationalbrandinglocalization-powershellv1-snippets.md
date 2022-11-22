---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	BackgroundColor = "#00000F"
	Id = "fr-FR"
	SignInPageText = " "
}

New-MgOrganizationBrandingLocalization -OrganizationId $organizationId -BodyParameter $params

```