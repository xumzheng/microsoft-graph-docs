---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "Sales department users"
	Description = "All users from sales department"
	AllowedTargetScope = "specificDirectoryUsers"
	SpecificAllowedTargets = @(
		@{
			"@odata.type" = "#microsoft.graph.attributeRuleMembers"
			Description = "Membership rule for all users from sales department"
			MembershipRule = "(user.department -eq "Sales")"
		}
	)
	AutomaticRequestSettings = @{
		RequestAccessForAllowedTargets = $true
	}
	AccessPackage = @{
		Id = "8a36831e-1527-4b2b-aff2-81259a8d8e76"
	}
}

New-MgEntitlementManagementAssignmentPolicy -BodyParameter $params

```