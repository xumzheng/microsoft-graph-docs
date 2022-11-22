---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	IsEnabled = "false"
}

Update-MgUserSettingItemInsight -UserId $userId -BodyParameter $params

```