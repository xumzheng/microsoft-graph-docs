---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	Message = @{
		Subject = "Meet for lunch?"
		Body = @{
			ContentType = "Text"
			Content = "The new cafeteria is open."
		}
		ToRecipients = @(
			@{
				EmailAddress = @{
					Address = "samanthab@contoso.onmicrosoft.com"
				}
			}
		)
		CcRecipients = @(
			@{
				EmailAddress = @{
					Address = "danas@contoso.onmicrosoft.com"
				}
			}
		)
	}
	SaveToSentItems = "false"
}

# A UPN can also be used as -UserId.
Send-MgBetaUserMail -UserId $userId -BodyParameter $params

```