---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Address = "Innocenty.Popov@adventureworks.com"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileEmail -UserId $userId -BodyParameter $params

```