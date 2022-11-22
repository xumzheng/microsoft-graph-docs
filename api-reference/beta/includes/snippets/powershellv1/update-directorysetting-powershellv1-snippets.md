---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	Values = @(
		@{
			Name = "CustomBlockedWordsList"
			Value = "Contoso"
		}
	)
}

Update-MgDirectorySetting -DirectorySettingId $directorySettingId -BodyParameter $params

```