---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	AuthoringLanguages = @(
		@{
			Locale = "en-US"
		}
		@{
			Locale = "es-MX"
		}
	)
	DefaultRegionalFormat = @{
		Locale = "en-US"
	}
}

# A UPN can also be used as -UserId.
Update-MgUserSettingRegionalAndLanguageSetting -UserId $userId -BodyParameter $params

```