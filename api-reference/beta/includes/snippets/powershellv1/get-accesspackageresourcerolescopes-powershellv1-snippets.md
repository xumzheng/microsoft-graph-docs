---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackage -AccessPackageId $accessPackageId -ExpandProperty "accessPackageResourceRoleScopes(`$expand=accessPackageResourceRole,accessPackageResourceScope)" 

```