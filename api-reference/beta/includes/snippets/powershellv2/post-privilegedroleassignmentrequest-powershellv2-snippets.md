---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Duration = "2"
	Reason = "Activate the role for business purpose"
	TicketNumber = "234"
	TicketSystem = "system"
	Schedule = @{
		StartDateTime = [System.DateTime]::Parse("2018-02-08T02:35:17.903Z")
	}
	Type = "UserAdd"
	AssignmentState = "Active"
	RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}

New-MgBetaPrivilegedRoleAssignmentRequest -BodyParameter $params

```