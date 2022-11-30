---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	AdditionalInformation = "additionalInformation-after-update"
	Confidence = 42
	Description = "description-after-update"
}

Update-MgBetaSecurityTiIndicator -TiIndicatorId $tiIndicatorId -BodyParameter $params

```