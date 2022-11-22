---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Categories = @(
		"Sports"
	)
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileInterest -UserId $userId -PersonInterestId $personInterestId -BodyParameter $params

```