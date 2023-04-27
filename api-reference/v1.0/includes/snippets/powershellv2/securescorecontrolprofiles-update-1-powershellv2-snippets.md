---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	assignedTo = ""
	comment = "control is reviewed"
	state = "Reviewed"
	vendorInformation = @{
		provider = "SecureScore"
		providerVersion = $null
		subProvider = $null
		vendor = "Microsoft"
	}
}

Update-MgSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```