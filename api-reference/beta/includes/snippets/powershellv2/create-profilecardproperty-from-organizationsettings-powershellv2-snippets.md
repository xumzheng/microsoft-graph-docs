---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	directoryPropertyName = "CustomAttribute1"
	annotations = @(
		@{
			displayName = "Cost Center"
			localizations = @(
				@{
					languageTag = "ru-RU"
					displayName = "центр затрат"
				}
			)
		}
	)
}

New-MgBetaOrganizationSettingProfileCardProperty -OrganizationId $organizationId -BodyParameter $params

```