---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.fileAssessmentRequest"
	expectedAssessment = "block"
	category = "malware"
	fileName = "test.txt"
	contentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```