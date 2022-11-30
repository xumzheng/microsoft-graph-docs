---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageAssignmentRequest -ExpandProperty "requestor(`$expand=connectedOrganization)" -Filter "(requestState eq 'PendingApproval')" 

```