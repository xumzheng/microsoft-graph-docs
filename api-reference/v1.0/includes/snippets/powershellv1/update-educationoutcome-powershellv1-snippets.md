---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Education

$params = @{
	"@odata.type" = "#microsoft.graph.educationRubricOutcome"
	RubricQualityFeedback = @(
	)
	RubricQualitySelectedLevels = @(
	)
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params

```