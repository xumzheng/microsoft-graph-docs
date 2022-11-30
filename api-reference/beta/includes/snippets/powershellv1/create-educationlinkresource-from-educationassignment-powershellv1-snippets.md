---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Education

$params = @{
	DistributeForStudentWork = $false
	Resource = @{
		DisplayName = "Where the Wonders of Learning Never Cease | Wonderopolis"
		Link = "https://wonderopolis.org/"
		ThumbnailPreviewUrl = $null
		"@odata.type" = "#microsoft.graph.educationLinkResource"
	}
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```