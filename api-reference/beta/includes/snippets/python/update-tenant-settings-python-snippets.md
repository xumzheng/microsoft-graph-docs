---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Settings();
requestBody.setDeletedUserPersonalSiteRetentionPeriodInDays(365);

requestBody.setExcludedFileExtensionsForSyncApp(['.mp3', ]);

requestBody.setImageTaggingOption(ImageTaggingChoice('enhanced'));

requestBody.setIsLegacyAuthProtocolsEnabled(true);

requestBody.setIsSitesStorageLimitAutomatic(false);

requestBody.setIsSyncButtonHiddenOnPersonalSite(false);

requestBody.setIsUnmanagedSyncAppForTenantRestricted(false);

requestBody.setPersonalSiteDefaultStorageLimitInMB(120000);



result = awaitclient.admin().sharepoint().settings().patch(requestBody);


```