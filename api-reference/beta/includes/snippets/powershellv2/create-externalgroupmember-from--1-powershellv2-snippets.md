---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Id = "e811976d-83df-4cbd-8b9b-5215b18aa874"
	Type = "user"
}

New-MgBetaExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```