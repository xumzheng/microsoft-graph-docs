---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	AccessPackageResourceRole = @{
		OriginId = "4"
		OriginSystem = "SharePointOnline"
		AccessPackageResource = @{
			Id = "53c71803-a0a8-4777-aecc-075de8ee3991"
		}
	}
	AccessPackageResourceScope = @{
		Id = "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
		OriginId = "https://microsoft.sharepoint.com/portals/Community"
		OriginSystem = "SharePointOnline"
	}
}

New-MgBetaEntitlementManagementAccessPackageResourceRoleScope -AccessPackageId $accessPackageId -BodyParameter $params

```