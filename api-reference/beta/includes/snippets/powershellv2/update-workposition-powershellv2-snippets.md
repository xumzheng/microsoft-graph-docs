---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	IsCurrent = $true
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfilePosition -UserId $userId -WorkPositionId $workPositionId -BodyParameter $params

```