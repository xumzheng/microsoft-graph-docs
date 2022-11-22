---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Education

$params = @{
	DistributeForStudentWork = $false
	Resource = @{
		DisplayName = "article.pdf"
		"@odata.type" = "#microsoft.graph.educationFileResource"
	}
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```