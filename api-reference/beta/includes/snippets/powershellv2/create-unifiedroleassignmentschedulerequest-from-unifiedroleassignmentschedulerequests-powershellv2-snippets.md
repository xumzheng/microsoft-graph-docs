---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Action = "AdminAssign"
	Justification = "Assign User Admin to IT Helpdesk (User) group"
	RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c"
	DirectoryScopeId = "/"
	PrincipalId = "07706ff1-46c7-4847-ae33-3003830675a1"
	ScheduleInfo = @{
		StartDateTime = [System.DateTime]::Parse("2021-07-01T00:00:00Z")
		Expiration = @{
			Type = "NoExpiration"
		}
	}
}

New-MgBetaRoleManagementDirectoryRoleAssignmentScheduleRequest -BodyParameter $params

```