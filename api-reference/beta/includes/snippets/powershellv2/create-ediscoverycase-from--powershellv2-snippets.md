---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	displayName = "CONTOSO LITIGATION-005"
	description = "Project Bazooka"
	externalId = "324516"
}

New-MgBetaSecurityCaseEdiscoveryCase -BodyParameter $params

```