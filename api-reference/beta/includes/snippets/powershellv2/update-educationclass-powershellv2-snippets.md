---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	Description = "History - World History 1"
	DisplayName = "World History Level 1"
}

Update-MgBetaEducationClass -EducationClassId $educationClassId -BodyParameter $params

```