---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	displayName = "Quizzes"
}

New-MgBetaEducationClassAssignmentCategory -EducationClassId $educationClassId -BodyParameter $params

```