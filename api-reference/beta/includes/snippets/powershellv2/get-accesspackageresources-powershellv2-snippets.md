---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

Get-MgBetaEntitlementManagementAccessPackageCatalogAccessPackageResource -AccessPackageCatalogId $accessPackageCatalogId -Filter "resourceType eq 'Application'" -ExpandProperty "accessPackageResourceScopes" 

```