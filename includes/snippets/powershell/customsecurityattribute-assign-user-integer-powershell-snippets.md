---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Users

$params = @{
	customSecurityAttributes = @{
		Engineering = @{
			"@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
			"NumVendors@odata.type" = "#Int32"
			NumVendors = 4
		}
	}
}

Update-MgUser -UserId $userId -BodyParameter $params

```