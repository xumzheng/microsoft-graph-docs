---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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


requestResult = graphServiceClient.directory().onPremisesSynchronizationById('onPremisesDirectorySynchronization-id').patch(requestBody);


```