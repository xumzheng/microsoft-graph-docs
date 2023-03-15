---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	MarketingNotificationEmails = @(
		"marketing@contoso.com"
	)
	PrivacyProfile = @{
		ContactEmail = "alice@contoso.com"
		StatementUrl = "https://contoso.com/privacyStatement"
	}
	SecurityComplianceNotificationMails = @(
		"security@contoso.com"
	)
	SecurityComplianceNotificationPhones = @(
		"(123) 456-7890"
	)
	TechnicalNotificationMails = @(
		"tech@contoso.com"
	)
}

Update-MgBetaOrganization -OrganizationId $organizationId -BodyParameter $params

```