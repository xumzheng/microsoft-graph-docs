---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Detail = @{
		Company = @{
			DisplayName = "Adventureworks Ltd."
			Department = "Consulting"
			OfficeLocation = "AW23/344"
			Address = @{
				Type = "business"
				Street = "123 Patriachy Ponds"
				City = "Moscow"
				CountryOrRegion = "Russian Federation"
				PostalCode = "RU-34621"
			}
			WebUrl = "https://www.adventureworks.com"
		}
		JobTitle = "Senior Product Branding Manager II"
		Role = "consulting"
	}
	IsCurrent = $true
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfilePosition -UserId $userId -BodyParameter $params

```