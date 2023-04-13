---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnPremisesDirectorySynchronization()
configuration = OnPremisesDirectorySynchronizationConfiguration()
configuration_accidental_deletion_prevention = OnPremisesAccidentalDeletionPrevention()
configurationAccidentalDeletionPrevention.SynchronizationPreventionType(OnPremisesDirectorySynchronizationDeletionPreventionType('enabledforcount'))

configurationAccidentalDeletionPrevention.alert_threshold = 500


configuration.accidental_deletion_prevention = configurationAccidentalDeletionPrevention

request_body.configuration = configuration
features = OnPremisesDirectorySynchronizationFeature()
features.group_write_back_enabled = True


request_body.features = features



result = await client.directory.onPremisesSynchronization_by_id('onPremisesDirectorySynchronization-id').patch(request_body = request_body)


```