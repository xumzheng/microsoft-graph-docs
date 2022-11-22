---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	AllowedAudiences = "organization"
}

Update-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId -BodyParameter $params

```