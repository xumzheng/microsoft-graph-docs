---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SharepointSettings()
request_body.deletedUserPersonalSiteRetentionPeriodInDays = 365

request_body.ExcludedFileExtensionsForSyncApp(['.mp3', ])

request_body.ImageTaggingOption(ImageTaggingChoice('enhanced'))

request_body.isLegacyAuthProtocolsEnabled = true

request_body.isSitesStorageLimitAutomatic = false

request_body.isSyncButtonHiddenOnPersonalSite = false

request_body.isUnmanagedSyncAppForTenantRestricted = false

request_body.personalSiteDefaultStorageLimitInMB = 120000




result = await client.admin.sharepoint.settings.patch(request_body = request_body)


```