---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	RegistrationEnforcement = @{
		AuthenticationMethodsRegistrationCampaign = @{
			SnoozeDurationInDays = 1
			State = "enabled"
			ExcludeTargets = @(
			)
			IncludeTargets = @(
				@{
					Id = "3ee3a9de-0a86-4e12-a287-9769accf1ba2"
					TargetType = "group"
					TargetedAuthenticationMethod = "microsoftAuthenticator"
				}
			)
		}
	}
}

Update-MgBetaPolicyAuthenticationMethodPolicy -BodyParameter $params

```