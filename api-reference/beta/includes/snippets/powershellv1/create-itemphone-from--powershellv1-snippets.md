---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	DisplayName = "Car Phone"
	Number = "+7 499 342 22 13"
}

# A UPN can also be used as -UserId.
New-MgUserProfilePhone -UserId $userId -BodyParameter $params

```