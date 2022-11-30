---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	Subject = "Shop for children's weekend"
	StartDateTime = @{
		DateTime = "2016-05-03T09:00:00"
		TimeZone = "Eastern Standard Time"
	}
	DueDateTime = @{
		DateTime = "2016-05-05T16:00:00"
		TimeZone = "Eastern Standard Time"
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserOutlookTask -UserId $userId -BodyParameter $params

```