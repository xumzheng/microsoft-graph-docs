---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	displayName = "Rogelio Cazares"
	givenName = "Rogelio"
	middleName = "Fernando"
	surname = "Cazares"
}

Update-MgBetaEducationUser -EducationUserId $educationUserId -BodyParameter $params

```