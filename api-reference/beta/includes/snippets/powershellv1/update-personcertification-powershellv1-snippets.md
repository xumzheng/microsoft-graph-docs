---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	IssuingAuthority = "International Academy of Marketing Excellence"
	IssuingCompany = "International Academy of Marketing Excellence"
}

Update-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId -BodyParameter $params

```