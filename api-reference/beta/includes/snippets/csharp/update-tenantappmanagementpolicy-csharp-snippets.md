---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TenantAppManagementPolicy
{
	IsEnabled = true,
	ApplicationRestrictions = new AppManagementConfiguration
	{
		PasswordCredentials = new List<PasswordCredentialConfiguration>
		{
			new PasswordCredentialConfiguration
			{
				RestrictionType = "passwordAddition",
				MaxLifetime = null,
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-01-01T10:37:00Z"),
			},
			new PasswordCredentialConfiguration
			{
				RestrictionType = "passwordLifetime",
				MaxLifetime = "P4DT12H30M5S",
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2017-01-01T10:37:00Z"),
			},
			new PasswordCredentialConfiguration
			{
				RestrictionType = "symmetricKeyAddition",
				MaxLifetime = null,
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-01-01T10:37:00Z"),
			},
			new PasswordCredentialConfiguration
			{
				RestrictionType = "customPasswordAddition",
				MaxLifetime = null,
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z"),
			},
			new PasswordCredentialConfiguration
			{
				RestrictionType = "symmetricKeyLifetime",
				MaxLifetime = "P40D",
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z"),
			},
		}
		KeyCredentials = new List<KeyCredentialConfiguration>
		{
			new KeyCredentialConfiguration
			{
				RestrictionType = "asymmetricKeyLifetime",
				MaxLifetime = "P30D",
				RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z"),
			},
		}
	},
};
await graphClient.Policies.DefaultAppManagementPolicy.PatchAsync(requestBody);


```