---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RetentionLabel();
$requestBody->set@odatatype('#microsoft.graph.security.retentionLabel');

$requestBody->setDisplayName('String');

$requestBody->setBehaviorDuringRetentionPeriod(new BehaviorDuringRetentionPeriod('string'));

$requestBody->setActionAfterRetentionPeriod(new ActionAfterRetentionPeriod('string'));

$requestBody->setRetentionTrigger(new RetentionTrigger('string'));

$retentionDuration = new RetentionDuration();
$retentionDuration->set@odatatype('microsoft.graph.security.retentionDuration');


$requestBody->setRetentionDuration($retentionDuration);
$requestBody->setIsInUse(boolean);

$requestBody->setDescriptionForAdmins('String');

$requestBody->setDescriptionForUsers('String');

$createdBy = new IdentitySet();
$createdBy->set@odatatype('microsoft.graph.identitySet');


$requestBody->setCreatedBy($createdBy);
$requestBody->setLabelToBeApplied('String');

$requestBody->setDefaultRecordBehavior(new DefaultRecordBehavior('string'));



$requestResult = $graphServiceClient->security()->labels()->retentionLabels()->post($requestBody);


```