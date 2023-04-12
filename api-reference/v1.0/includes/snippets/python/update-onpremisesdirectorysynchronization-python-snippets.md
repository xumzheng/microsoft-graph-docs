---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnPremisesDirectorySynchronization()
configuration = OnPremisesDirectorySynchronizationConfiguration()
configurationAccidentalDeletionPrevention = OnPremisesAccidentalDeletionPrevention()
configurationAccidentalDeletionPrevention.SynchronizationPreventionType(OnPremisesDirectorySynchronizationDeletionPreventionType('enabledforcount'))

configurationAccidentalDeletionPrevention.alertThreshold = 500


configuration.accidentalDeletionPrevention = configurationAccidentalDeletionPrevention

request_body.configuration = configuration
features = OnPremisesDirectorySynchronizationFeature()
features.groupWriteBackEnabled = true


request_body.features = features



result = await client.directory.onPremisesSynchronization_by_id('onPremisesDirectorySynchronization-id').patch(request_body = request_body)


```