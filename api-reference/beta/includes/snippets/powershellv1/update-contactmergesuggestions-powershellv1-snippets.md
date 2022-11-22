---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	IsEnabled = $false
}

# A UPN can also be used as -UserId.
Update-MgUserSettingContactMergeSuggestion -UserId $userId -BodyParameter $params

```