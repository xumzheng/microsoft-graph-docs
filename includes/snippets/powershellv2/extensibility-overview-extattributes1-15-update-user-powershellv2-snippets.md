---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

$params = @{
	onPremisesExtensionAttributes = @{
		extensionAttribute1 = "skypeId.adeleVance"
		extensionAttribute13 = $null
	}
}

Update-MgUser -UserId $userId -BodyParameter $params

```