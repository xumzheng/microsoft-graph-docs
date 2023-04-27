---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Search

$params = @{
	id = "contosohr"
	name = "Contoso HR"
	description = "Connection to index Contoso HR system"
}

New-MgExternalConnection -BodyParameter $params

```