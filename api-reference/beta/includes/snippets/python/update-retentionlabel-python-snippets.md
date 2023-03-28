---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RetentionLabel();
$requestBody.set@odatatype('#microsoft.graph.security.retentionLabel');

$retentionDuration = new RetentionDuration();
$retentionDuration.set@odatatype('microsoft.graph.security.retentionDuration');


$requestBody.setRetentionDuration($retentionDuration);
$requestBody.setDescriptionForAdmins('String');

$requestBody.setDescriptionForUsers('String');

$requestBody.setLabelToBeApplied('String');

$requestBody.setDefaultRecordBehavior(new DefaultRecordBehavior('string'));



$requestResult = $graphServiceClient.security().labels().retentionLabelsById('retentionLabel-id').patch($requestBody);


```