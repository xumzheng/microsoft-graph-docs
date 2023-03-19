---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	Message = @{
		Subject = "Project kickoff"
		ToRecipients = @(
			@{
				EmailAddress = @{
					Name = "Samantha Booth"
					Address = "samanthab@contoso.onmicrosoft.com"
				}
			}
		)
		Mentions = @(
			@{
				Mentioned = @{
					Name = "Dana Swope"
					Address = "danas@contoso.onmicrosoft.com"
				}
			}
		)
	}
}

# A UPN can also be used as -UserId.
Send-MgBetaUserMail -UserId $userId -BodyParameter $params

```