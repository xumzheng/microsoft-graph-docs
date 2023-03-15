---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Description = "Contoso Life v2.0"
	DisplayName = "Contoso Life Renewed"
}

Update-MgBetaGroup -GroupId $groupId -BodyParameter $params

```