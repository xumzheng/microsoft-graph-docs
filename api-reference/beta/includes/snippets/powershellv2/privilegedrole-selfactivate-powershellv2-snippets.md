---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Reason = "reason-value"
	Duration = "duration-value"
	TicketNumber = "ticketNumber-value"
	TicketSystem = "ticketSystem-value"
}

Invoke-MgBetaSelfPrivilegedRoleActivate -PrivilegedRoleId $privilegedRoleId -BodyParameter $params

```