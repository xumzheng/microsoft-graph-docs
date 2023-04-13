---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SharepointSettings()
request_body.deleted_user_personal_site_retention_period_in_days = 365

request_body.ExcludedFileExtensionsForSyncApp(['.mp3', ])

request_body.ImageTaggingOption(ImageTaggingChoice('enhanced'))

request_body.is_legacy_auth_protocols_enabled = True

request_body.is_sites_storage_limit_automatic = False

request_body.is_sync_button_hidden_on_personal_site = False

request_body.is_unmanaged_sync_app_for_tenant_restricted = False

request_body.personal_site_default_storage_limit_in_m_b = 120000




result = await client.admin.sharepoint.settings.patch(request_body = request_body)


```