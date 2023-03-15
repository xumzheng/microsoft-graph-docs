---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	DistributeForStudentWork = $false
	Resource = @{
		DisplayName = "article.pdf"
		"@odata.type" = "#microsoft.graph.educationFileResource"
	}
}

New-MgBetaEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```