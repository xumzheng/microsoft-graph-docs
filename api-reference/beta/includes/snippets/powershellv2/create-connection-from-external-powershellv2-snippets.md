---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	id = "contosohr"
	name = "Contoso HR"
	description = "Connection to index Contoso HR system"
}

New-MgBetaExternalConnection -BodyParameter $params

```