---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	customSecurityAttributes = @{
		Engineering = @{
			"@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
			ProjectDate = "2022-10-01"
		}
	}
}

Update-MgBetaServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```