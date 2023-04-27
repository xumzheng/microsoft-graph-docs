---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	customSecurityAttributes = @{
		Engineering = @{
			"@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
			Certification = $false
		}
	}
}

Update-MgBetaUser -UserId $userId -BodyParameter $params

```