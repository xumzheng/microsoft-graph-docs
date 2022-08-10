---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Organization
{
	MarketingNotificationEmails = new List<>
	{
		"marketing@contoso.com",
	},
	PrivacyProfile = new PrivacyProfile
	{
		ContactEmail = "alice@contoso.com",
		StatementUrl = "https://contoso.com/privacyStatement",
	},
	SecurityComplianceNotificationMails = new List<>
	{
		"security@contoso.com",
	},
	SecurityComplianceNotificationPhones = new List<>
	{
		"(123) 456-7890",
	},
	TechnicalNotificationMails = new List<>
	{
		"tech@contoso.com",
	},
};
await graphClient.Organization["organization-id"].PatchAsync(requestBody);


```