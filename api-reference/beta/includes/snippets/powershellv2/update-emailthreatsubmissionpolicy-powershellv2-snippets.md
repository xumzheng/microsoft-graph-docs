---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	isReportToMicrosoftEnabled = $false
}

Update-MgBetaSecurityThreatSubmissionEmailThreatSubmissionPolicy -EmailThreatSubmissionPolicyId $emailThreatSubmissionPolicyId -BodyParameter $params

```