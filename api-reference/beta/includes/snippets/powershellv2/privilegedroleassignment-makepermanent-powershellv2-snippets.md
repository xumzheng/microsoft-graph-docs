---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Reason = "reason-value"
	TicketNumber = "ticketNumber-value"
	TicketSystem = "ticketSystem-value"
}

New-MgBetaPrivilegedRoleAssignmentPermanent -PrivilegedRoleAssignmentId $privilegedRoleAssignmentId -BodyParameter $params

```