---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "#microsoft.graph.urlThreatSubmission"
	Category = "phishing"
	WebUrl = "http://phishing.contoso.com"
}

New-MgBetaSecurityThreatSubmissionUrlThreat -BodyParameter $params

```