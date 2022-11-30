---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	IsEnabled = "false"
}

Update-MgBetaUserSettingItemInsight -UserId $userId -BodyParameter $params

```