---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Education

$params = @{
	submissionAnimationDisabled = $true
}

Update-MgEducationClassAssignmentSetting -EducationClassId $educationClassId -BodyParameter $params

```