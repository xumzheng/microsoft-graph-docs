---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	displayName = "Example Credit Rubric after display name patch"
}

Update-MgBetaEducationMeRubric -EducationRubricId $educationRubricId -BodyParameter $params

```