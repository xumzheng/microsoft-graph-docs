---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	BusinessPhones = @(
		"+1 425 555 0109"
	)
	OfficeLocation = "18/2111"
	AuthorizationInfo = @{
		CertificateUserIds = @(
			"5432109876543210@mil"
		)
	}
}

Update-MgBetaUser -UserId $userId -BodyParameter $params

```