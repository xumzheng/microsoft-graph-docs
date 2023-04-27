---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
	securityEnabledOnly = $false
}

Get-MgDirectoryObjectMemberGroup -DirectoryObjectId $directoryObjectId -BodyParameter $params

```