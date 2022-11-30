---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	CustomSecurityAttributes = @{
		Engineering = @{
			"@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
			"Project@odata.type" = "#Collection(String)"
			Project = @(
				"Baker"
				"Cascade"
			)
		}
	}
}

Update-MgBetaUser -UserId $userId -BodyParameter $params

```