---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	EmailAddress = "kim@contoso.com"
}

New-MgBetaUserAuthenticationEmailMethod -UserId $userId -BodyParameter $params

```