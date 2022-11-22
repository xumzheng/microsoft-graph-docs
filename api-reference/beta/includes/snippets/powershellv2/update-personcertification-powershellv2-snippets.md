---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	IssuingAuthority = "International Academy of Marketing Excellence"
	IssuingCompany = "International Academy of Marketing Excellence"
}

Update-MgBetaUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId -BodyParameter $params

```