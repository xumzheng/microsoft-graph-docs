---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	SkuId = "6fd2c87f-b296-42f0-b197-1e91e994b900"
	ServicePlanId = "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}

Initialize-MgBetaOrganizationService -OrganizationId $organizationId -BodyParameter $params

```