---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	ClassifyAs = "focused"
	SenderEmailAddress = @{
		Name = "Samantha Booth"
		Address = "samanthab@adatum.onmicrosoft.com"
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserInferenceClassificationOverride -UserId $userId -BodyParameter $params

```