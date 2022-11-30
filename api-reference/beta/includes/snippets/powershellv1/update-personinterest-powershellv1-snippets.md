---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	Categories = @(
		"Sports"
	)
}

# A UPN can also be used as -UserId.
Update-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId -BodyParameter $params

```