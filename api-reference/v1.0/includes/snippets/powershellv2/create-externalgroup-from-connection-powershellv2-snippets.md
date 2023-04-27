---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Search

$params = @{
	id = "31bea3d537902000"
	displayName = "Contoso Marketing"
	description = "The product marketing team"
}

New-MgExternalConnectionGroup -ExternalConnectionId $externalConnectionId -BodyParameter $params

```