---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Name = "Contoso HR Service Tickets"
	Description = "Connection to index HR service tickets"
}

Update-MgBetaExternalConnection -ExternalConnectionId $externalConnectionId -BodyParameter $params

```