---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	"@odata.type" = "#microsoft.graph.educationFeedbackResourceOutcome"
	FeedbackResource = @{
		"@odata.type" = "#microsoft.graph.educationWordResource"
		DisplayName = "Document1.docx"
	}
}

New-MgBetaEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```