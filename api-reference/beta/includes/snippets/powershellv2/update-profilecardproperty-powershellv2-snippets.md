---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	Annotations = @(
		@{
			Localizations = @(
				@{
					LanguageTag = "no-NB"
					DisplayName = "Kostnads Senter"
				}
			)
		}
	)
}

Update-MgBetaOrganizationSettingProfileCardProperty -OrganizationId $organizationId -ProfileCardPropertyId $profileCardPropertyId -BodyParameter $params

```