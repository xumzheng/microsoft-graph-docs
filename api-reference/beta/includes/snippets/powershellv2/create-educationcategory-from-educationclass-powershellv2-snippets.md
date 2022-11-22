---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	DisplayName = "Quizzes"
}

New-MgBetaEducationClassAssignmentCategory -EducationClassId $educationClassId -BodyParameter $params

```