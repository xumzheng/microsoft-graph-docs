---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	NewPassword = "Cuyo5459"
}

Reset-MgUserAuthenticationMethodPassword -UserId $userId -AuthenticationMethodId $authenticationMethodId -BodyParameter $params

```