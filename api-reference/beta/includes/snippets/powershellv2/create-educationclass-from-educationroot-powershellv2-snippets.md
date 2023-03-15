---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	Description = "Health Level 1"
	ClassCode = "Health 501"
	DisplayName = "Health 1"
	ExternalId = "11019"
	ExternalName = "Health Level 1"
	ExternalSource = "sis"
	MailNickname = "fineartschool.net"
}

New-MgBetaEducationClass -BodyParameter $params

```