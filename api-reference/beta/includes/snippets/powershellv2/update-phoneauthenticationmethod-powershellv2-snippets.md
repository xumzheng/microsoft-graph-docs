---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	PhoneNumber = "+1 2065555554"
	PhoneType = "mobile"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserAuthenticationPhoneMethod -UserId $userId -PhoneAuthenticationMethodId $phoneAuthenticationMethodId -BodyParameter $params

```