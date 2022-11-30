---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

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

New-MgOrganizationSettingProfileCardProperty -OrganizationId $organizationId -BodyParameter $params

```