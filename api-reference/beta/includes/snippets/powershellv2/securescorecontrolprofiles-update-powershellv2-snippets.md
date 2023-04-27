---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	controlStateUpdates = "controlStateUpdates-value"
}

Update-MgBetaSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```