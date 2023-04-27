---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Education

$params = @{
	addedStudentAction = "assignIfOpen"
	addToCalendarAction = "studentsAndTeamOwners"
	notificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}

Update-MgBetaEducationClassAssignmentDefault -EducationClassId $educationClassId -BodyParameter $params

```