---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	Subject = "subject-value"
	Body = @{
		ContentType = ""
		Content = "content-value"
	}
	InferenceClassification = "other"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```