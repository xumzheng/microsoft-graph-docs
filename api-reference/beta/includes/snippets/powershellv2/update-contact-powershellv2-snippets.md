---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.PersonalContacts

$params = @{
	EmailAddresses = @(
		@{
			Type = "personal"
			Name = "Pavel Bansky"
			Address = "pavelb@adatum.onmicrosoft.com"
		}
		@{
			Address = "pavelb@fabrikam.onmicrosoft.com"
			Name = "Pavel Bansky"
			Type = "other"
			OtherLabel = "Volunteer work"
		}
	)
}

# A UPN can also be used as -UserId.
Update-MgBetaUserContact -UserId $userId -ContactId $contactId -BodyParameter $params

```