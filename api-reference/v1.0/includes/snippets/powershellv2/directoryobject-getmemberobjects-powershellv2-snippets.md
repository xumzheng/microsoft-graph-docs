---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
	securityEnabledOnly = $true
}

Get-MgDirectoryObjectMemberObject -DirectoryObjectId $directoryObjectId -BodyParameter $params

```