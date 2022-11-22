---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Education

$params = @{
	SubmissionAnimationDisabled = $true
}

Update-MgEducationClassAssignmentSetting -EducationClassId $educationClassId -BodyParameter $params

```