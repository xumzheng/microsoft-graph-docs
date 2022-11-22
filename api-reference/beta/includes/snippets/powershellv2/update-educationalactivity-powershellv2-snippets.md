---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Institution = @{
		Location = @{
			Type = "business"
			PostOfficeBox = $null
			Street = "12000 E Prospect Rd"
			City = "Fort Collins"
			State = "Colorado"
			CountryOrRegion = "USA"
			PostalCode = "80525"
		}
	}
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId -BodyParameter $params

```