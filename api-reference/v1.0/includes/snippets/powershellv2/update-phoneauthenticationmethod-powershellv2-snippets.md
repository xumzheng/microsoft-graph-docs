---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	phoneNumber = "+1 2065555554"
	phoneType = "mobile"
}

# A UPN can also be used as -UserId.
Update-MgUserAuthenticationPhoneMethod -UserId $userId -PhoneAuthenticationMethodId $phoneAuthenticationMethodId -BodyParameter $params

```