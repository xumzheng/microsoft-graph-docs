---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	MemberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33"
	MembershipRule = "(user.displayName -startsWith "EndTestUser")"
}

Test-MgBetaGroupDynamicMembershipRule -BodyParameter $params

```