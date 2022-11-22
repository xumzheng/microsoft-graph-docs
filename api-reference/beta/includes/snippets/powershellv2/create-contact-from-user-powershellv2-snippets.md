---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.PersonalContacts

$params = @{
	GivenName = "Pavel"
	Surname = "Bansky"
	EmailAddresses = @(
		@{
			Address = "pavelb@contoso.onmicrosoft.com"
			Name = "Pavel Bansky"
			Type = "personal"
		}
		@{
			Address = "pavelb@fabrikam.onmicrosoft.com"
			Name = "Pavel Bansky"
			Type = "other"
			OtherLabel = "Volunteer work"
		}
	)
	Phones = @(
		@{
			Number = "+1 732 555 0102"
			Type = "business"
		}
	)
}

# A UPN can also be used as -UserId.
New-MgBetaUserContact -UserId $userId -BodyParameter $params

```