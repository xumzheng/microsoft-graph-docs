---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Description = "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel."
	DisplayName = "Inferring User Intent through browsing behaviors"
	IsPending = $true
	Number = "USPTO-3954432633"
	WebUrl = "https://patents.gov/3954432633"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfilePatent -UserId $userId -BodyParameter $params

```