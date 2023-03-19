---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	SubmissionAnimationDisabled = $true
}

Update-MgBetaEducationClassAssignmentSetting -EducationClassId $educationClassId -BodyParameter $params

```