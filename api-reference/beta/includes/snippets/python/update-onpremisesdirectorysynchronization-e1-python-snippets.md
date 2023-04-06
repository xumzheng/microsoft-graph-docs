---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnPremisesDirectorySynchronization()
configuration = OnPremisesDirectorySynchronizationConfiguration()
configurationAccidentalDeletionPrevention = OnPremisesAccidentalDeletionPrevention()
configurationAccidentalDeletionPrevention.setSynchronizationPreventionType(OnPremisesDirectorySynchronizationDeletionPreventionType('enabledforcount'))

configurationAccidentalDeletionPrevention.setAlertThreshold(500)


configuration.setAccidentalDeletionPrevention($configurationAccidentalDeletionPrevention)
$configuration.setSynchronizationInterval( \DateInterval('PT30M'))

$configuration.setCustomerRequestedSynchronizationInterval( \DateInterval('PT1H'))


request_body.setConfiguration($configuration)
features = OnPremisesDirectorySynchronizationFeature()
features.setGroupWriteBackEnabled(true)


request_body.setFeatures($features)

request_config = OnPremisesDirectorySynchronizationRequestBuilderPatchRequestConfiguration(
request_config = OnPremisesDirectorySynchronizationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.directory.onPremisesSynchronization_by_id('onPremisesDirectorySynchronization-id').patch(request_body, headers=)


```