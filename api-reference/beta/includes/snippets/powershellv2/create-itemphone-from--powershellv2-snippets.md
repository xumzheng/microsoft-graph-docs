---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	DisplayName = "Car Phone"
	Number = "+7 499 342 22 13"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfilePhone -UserId $userId -BodyParameter $params

```