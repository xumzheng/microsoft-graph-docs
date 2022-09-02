---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..TenantAdmin.Settings
{
	DeletedUserPersonalSiteRetentionPeriodInDays = 365,
	ExcludedFileExtensionsForSyncApp = new List<string>
	{
		".mp3",
	},
	ImageTaggingOption = ImageTaggingChoice.Enhanced,
	IsLegacyAuthProtocolsEnabled = true,
	IsSitesStorageLimitAutomatic = false,
	IsSyncButtonHiddenOnPersonalSite = false,
	IsUnmanagedSyncAppForTenantRestricted = false,
	PersonalSiteDefaultStorageLimitInMB = 120000L,
};
await graphClient.Admin.Sharepoint.Settings.PatchAsync(requestBody);


```