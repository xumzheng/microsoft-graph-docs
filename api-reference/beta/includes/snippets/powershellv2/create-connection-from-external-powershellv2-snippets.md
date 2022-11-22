---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Id = "contosohr"
	Name = "Contoso HR"
	Description = "Connection to index Contoso HR system"
}

New-MgBetaExternalConnection -BodyParameter $params

```