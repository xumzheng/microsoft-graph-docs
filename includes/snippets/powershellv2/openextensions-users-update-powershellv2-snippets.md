---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

$params = @{
	Theme = "light"
	Color = "yellow"
	Lang = "Swahili"
}

# A UPN can also be used as -UserId.
Update-MgUserExtension -UserId $userId -ExtensionId $extensionId -BodyParameter $params

```