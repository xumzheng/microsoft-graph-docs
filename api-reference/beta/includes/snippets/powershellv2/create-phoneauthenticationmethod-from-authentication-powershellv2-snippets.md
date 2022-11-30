---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	PhoneNumber = "+1 2065555555"
	PhoneType = "mobile"
}

# A UPN can also be used as -UserId.
New-MgBetaUserAuthenticationPhoneMethod -UserId $userId -BodyParameter $params

```