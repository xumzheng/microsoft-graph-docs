---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	AdminEligibleSettings = @(
		@{
			RuleIdentifier = "ExpirationRule"
			Setting = "{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}"
		}
	)
}

Update-MgBetaPrivilegedAccessRoleSetting -PrivilegedAccessId $privilegedAccessId -GovernanceRoleSettingId $governanceRoleSettingId -BodyParameter $params

```