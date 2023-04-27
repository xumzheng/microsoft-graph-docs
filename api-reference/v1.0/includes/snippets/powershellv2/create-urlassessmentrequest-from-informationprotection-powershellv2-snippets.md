---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.urlAssessmentRequest"
	url = "http://test.com"
	expectedAssessment = "block"
	category = "phishing"
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```