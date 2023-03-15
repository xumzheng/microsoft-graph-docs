---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.countryNamedLocation"
	DisplayName = "Named location with unknown countries and regions"
	CountriesAndRegions = @(
		"US"
		"GB"
	)
	IncludeUnknownCountriesAndRegions = $true
}

New-MgIdentityConditionalAccessNamedLocation -BodyParameter $params

```