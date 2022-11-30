---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/education/classes/11006"
}

New-MgBetaEducationSchoolClassByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```