---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	Subject = "9/8/2018: concert"
	Body = @{
		ContentType = "HTML"
		Content = "The group represents Washington."
	}
	ToRecipients = @(
		@{
			EmailAddress = @{
				Address = "AlexW@contoso.OnMicrosoft.com"
			}
		}
	)
	InternetMessageHeaders = @(
		@{
			Name = "x-custom-header-group-name"
			Value = "Washington"
		}
		@{
			Name = "x-custom-header-group-id"
			Value = "WA001"
		}
	)
}

# A UPN can also be used as -UserId.
New-MgBetaUserMessage -UserId $userId -BodyParameter $params

```