---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6"
	Proof = "eyJ0eXAiOiJ..."
}

Remove-MgBetaApplicationKey -ApplicationId $applicationId -BodyParameter $params

```