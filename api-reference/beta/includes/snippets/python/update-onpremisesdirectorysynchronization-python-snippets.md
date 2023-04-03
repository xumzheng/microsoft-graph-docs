---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OnPremisesDirectorySynchronization();
configuration = OnPremisesDirectorySynchronizationConfiguration();
configurationAccidentalDeletionPrevention = OnPremisesAccidentalDeletionPrevention();
configurationAccidentalDeletionPrevention.setSynchronizationPreventionType(OnPremisesDirectorySynchronizationDeletionPreventionType('enabledforcount'));

configurationAccidentalDeletionPrevention.setAlertThreshold(500);


configuration.setAccidentalDeletionPrevention($configurationAccidentalDeletionPrevention);

requestBody.setConfiguration($configuration);
features = OnPremisesDirectorySynchronizationFeature();
features.setGroupWriteBackEnabled(true);


requestBody.setFeatures($features);


result = await client.directory().onPremisesSynchronizationById('onPremisesDirectorySynchronization-id').patch(requestBody);


```