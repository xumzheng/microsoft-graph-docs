---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	emailAddress = "kim@contoso.com"
}

New-MgUserAuthenticationEmailMethod -UserId $userId -BodyParameter $params

```