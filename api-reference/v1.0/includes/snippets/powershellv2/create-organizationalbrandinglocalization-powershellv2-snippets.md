---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	backgroundColor = "#00000F"
	id = "fr-FR"
	signInPageText = " "
}

New-MgOrganizationBrandingLocalization -OrganizationId $organizationId -BodyParameter $params

```