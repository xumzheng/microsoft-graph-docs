---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Settings();
$requestBody.setDeletedUserPersonalSiteRetentionPeriodInDays(365);

$requestBody.setExcludedFileExtensionsForSyncApp(['.mp3', ]);

$requestBody.setImageTaggingOption(new ImageTaggingChoice('enhanced'));

$requestBody.setIsLegacyAuthProtocolsEnabled(true);

$requestBody.setIsSitesStorageLimitAutomatic(false);

$requestBody.setIsSyncButtonHiddenOnPersonalSite(false);

$requestBody.setIsUnmanagedSyncAppForTenantRestricted(false);

$requestBody.setPersonalSiteDefaultStorageLimitInMB(120000);



$requestResult = $graphServiceClient.admin().sharepoint().settings().patch($requestBody);


```