---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Security

$params = @{
	IsReportToMicrosoftEnabled = $false
}

Update-MgSecurityThreatSubmissionEmailThreatSubmissionPolicy -EmailThreatSubmissionPolicyId $emailThreatSubmissionPolicyId -BodyParameter $params

```