---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

Get-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -UnifiedRoleAssignmentScheduleRequestId $unifiedRoleAssignmentScheduleRequestId -Property "principalId,action,roleDefinitionId" -ExpandProperty "roleDefinition,activatedUsing,principal,targetSchedule" 

```