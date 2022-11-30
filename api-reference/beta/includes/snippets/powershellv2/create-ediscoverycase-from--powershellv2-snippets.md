---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	DisplayName = "CONTOSO LITIGATION-005"
	Description = "Project Bazooka"
	ExternalId = "324516"
}

New-MgBetaSecurityCaseEdiscoveryCase -BodyParameter $params

```