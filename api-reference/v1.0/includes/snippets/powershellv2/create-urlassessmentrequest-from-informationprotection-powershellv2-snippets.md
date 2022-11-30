---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.urlAssessmentRequest"
	Url = "http://test.com"
	ExpectedAssessment = "block"
	Category = "phishing"
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```