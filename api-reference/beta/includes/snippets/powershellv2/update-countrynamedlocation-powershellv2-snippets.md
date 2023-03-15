---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.countryNamedLocation"
	DisplayName = "Updated named location without unknown countries and regions"
	CountriesAndRegions = @(
		"CA"
		"IN"
	)
	IncludeUnknownCountriesAndRegions = $false
}

Update-MgBetaIdentityConditionalAccessNamedLocation -NamedLocationId $namedLocationId -BodyParameter $params

```