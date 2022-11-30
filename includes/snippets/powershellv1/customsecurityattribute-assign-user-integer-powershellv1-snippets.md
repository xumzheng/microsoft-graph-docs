---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	CustomSecurityAttributes = @{
		Engineering = @{
			"@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
			"NumVendors@odata.type" = "#Int32"
			NumVendors = 
		}
	}
}

Update-MgUser -UserId $userId -BodyParameter $params

```