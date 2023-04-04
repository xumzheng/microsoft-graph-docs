---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Settings();
request_body.setDeletedUserPersonalSiteRetentionPeriodInDays(365);

request_body.setExcludedFileExtensionsForSyncApp(['.mp3', ]);

request_body.setImageTaggingOption(ImageTaggingChoice('enhanced'));

request_body.setIsLegacyAuthProtocolsEnabled(true);

request_body.setIsSitesStorageLimitAutomatic(false);

request_body.setIsSyncButtonHiddenOnPersonalSite(false);

request_body.setIsUnmanagedSyncAppForTenantRestricted(false);

request_body.setPersonalSiteDefaultStorageLimitInMB(120000);



result = await client.admin.sharepoint.settings.patch(request_body);


```