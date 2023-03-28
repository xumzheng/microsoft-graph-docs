---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OnPremisesDirectorySynchronization();
$configuration = new OnPremisesDirectorySynchronizationConfiguration();
$configurationAccidentalDeletionPrevention = new OnPremisesAccidentalDeletionPrevention();
$configurationAccidentalDeletionPrevention->setSynchronizationPreventionType(new OnPremisesDirectorySynchronizationDeletionPreventionType('enabledforcount'));

$configurationAccidentalDeletionPrevention->setAlertThreshold(500);


$configuration->setAccidentalDeletionPrevention($configurationAccidentalDeletionPrevention);

$requestBody->setConfiguration($configuration);
$features = new OnPremisesDirectorySynchronizationFeature();
$features->setGroupWriteBackEnabled(true);


$requestBody->setFeatures($features);


$requestResult = $graphServiceClient->directory()->onPremisesSynchronizationById('onPremisesDirectorySynchronization-id')->patch($requestBody);


```