---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/education/users/14008"
}

New-MgBetaEducationSchoolUserByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```