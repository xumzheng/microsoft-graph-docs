---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	StartDateTime = [System.DateTime]::Parse("2022-06-05T00:00:00.000Z")
	LifetimeInMinutes = 60
	IsUsableOnce = $false
}

New-MgBetaUserAuthenticationTemporaryAccessPassMethod -UserId $userId -BodyParameter $params

```