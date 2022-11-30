---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	CatalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5"
	RequestType = "AdminAdd"
	Justification = ""
	AccessPackageResource = @{
		DisplayName = "Sales"
		Description = "https://contoso.sharepoint.com/sites/Sales"
		Url = "https://contoso.sharepoint.com/sites/Sales"
		ResourceType = "SharePoint Online Site"
		OriginId = "https://contoso.sharepoint.com/sites/Sales"
		OriginSystem = "SharePointOnline"
	}
}

New-MgBetaEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```