---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	DisplayName = "CN=customDisplayName"
	EndDateTime = [System.DateTime]::Parse("2024-01-25T00:00:00Z")
}

Add-MgBetaServicePrincipalTokenSigningCertificate -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```