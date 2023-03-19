---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	DisplayName = "Home"
	Detail = @{
		Type = "home"
		PostOfficeBox = $null
		Street = "221B Baker Street"
		City = "London"
		State = $null
		CountryOrRegion = "United Kingdom"
		PostalCode = "E14 3TD"
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileAddress -UserId $userId -BodyParameter $params

```