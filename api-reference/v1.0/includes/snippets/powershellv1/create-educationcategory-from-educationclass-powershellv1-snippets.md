---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Education

$params = @{
	DisplayName = "Quizzes"
}

New-MgEducationClassAssignmentCategory -EducationClassId $educationClassId -BodyParameter $params

```