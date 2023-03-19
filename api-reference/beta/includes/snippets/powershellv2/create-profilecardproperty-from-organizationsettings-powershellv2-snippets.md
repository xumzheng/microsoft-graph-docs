---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	DirectoryPropertyName = "CustomAttribute1"
	Annotations = @(
		@{
			DisplayName = "Cost Center"
			Localizations = @(
				@{
					LanguageTag = "ru-RU"
					DisplayName = "центр затрат"
				}
			)
		}
	)
}

New-MgBetaOrganizationSettingProfileCardProperty -OrganizationId $organizationId -BodyParameter $params

```