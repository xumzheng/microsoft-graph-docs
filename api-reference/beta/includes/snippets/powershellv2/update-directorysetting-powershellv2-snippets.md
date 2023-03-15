---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	Values = @(
		@{
			Name = "CustomBlockedWordsList"
			Value = "Contoso"
		}
	)
}

Update-MgBetaDirectorySetting -DirectorySettingId $directorySettingId -BodyParameter $params

```