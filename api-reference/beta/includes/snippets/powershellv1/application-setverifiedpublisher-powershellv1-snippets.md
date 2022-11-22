---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	VerifiedPublisherId = "1234567"
}

Set-MgApplicationVerifiedPublisher -ApplicationId $applicationId -BodyParameter $params

```