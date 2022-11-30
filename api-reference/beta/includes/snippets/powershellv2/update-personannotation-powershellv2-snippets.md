---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	AllowedAudiences = "organization"
}

Update-MgBetaUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId -BodyParameter $params

```