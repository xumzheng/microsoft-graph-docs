---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	OnPremisesPublishing = @{
		ExternalAuthenticationType = "aadPreAuthentication"
		InternalUrl = "https://contosoiwaapp.com"
		ExternalUrl = "https://contosoiwaapp-contoso.msappproxy.net"
		IsHttpOnlyCookieEnabled = $true
		IsOnPremPublishingEnabled = $true
		IsPersistentCookieEnabled = $true
		IsSecureCookieEnabled = $true
		IsStateSessionEnabled = $true
		IsTranslateHostHeaderEnabled = $true
		IsTranslateLinksInBodyEnabled = $true
	}
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```