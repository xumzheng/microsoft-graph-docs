---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Security

$params = @{
	"@odata.type" = "#microsoft.graph.urlThreatSubmission"
	Category = "phishing"
	WebUrl = "http://phishing.contoso.com"
}

New-MgSecurityThreatSubmissionUrlThreat -BodyParameter $params

```