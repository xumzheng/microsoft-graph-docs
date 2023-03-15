---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.countryNamedLocation"
	DisplayName = "Named location with unknown countries and regions"
	CountriesAndRegions = @(
		"US"
		"GB"
	)
	IncludeUnknownCountriesAndRegions = $true
}

New-MgBetaIdentityConditionalAccessNamedLocation -BodyParameter $params

```