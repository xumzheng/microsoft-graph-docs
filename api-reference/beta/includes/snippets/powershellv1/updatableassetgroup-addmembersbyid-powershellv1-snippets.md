---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
	Ids = @(
		"String"
		"String"
		"String"
	)
	MemberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice"
}

Add-MgWindowsUpdatesUpdatableAssetMemberById -UpdatableAssetId $updatableAssetId -BodyParameter $params

```