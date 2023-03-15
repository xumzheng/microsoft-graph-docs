---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	IsEnabled = $false
}

# A UPN can also be used as -UserId.
Update-MgBetaUserSettingContactMergeSuggestion -UserId $userId -BodyParameter $params

```