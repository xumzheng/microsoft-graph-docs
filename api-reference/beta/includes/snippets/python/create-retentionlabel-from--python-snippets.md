---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RetentionLabel();
requestBody.set@odatatype('#microsoft.graph.security.retentionLabel');

requestBody.setDisplayName('String');

requestBody.setBehaviorDuringRetentionPeriod(BehaviorDuringRetentionPeriod('string'));

requestBody.setActionAfterRetentionPeriod(ActionAfterRetentionPeriod('string'));

requestBody.setRetentionTrigger(RetentionTrigger('string'));

retentionDuration = RetentionDuration();
retentionDuration.set@odatatype('microsoft.graph.security.retentionDuration');


requestBody.setRetentionDuration($retentionDuration);
requestBody.setIsInUse(boolean);

requestBody.setDescriptionForAdmins('String');

requestBody.setDescriptionForUsers('String');

createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);
requestBody.setLabelToBeApplied('String');

requestBody.setDefaultRecordBehavior(DefaultRecordBehavior('string'));



result = await client.security().labels().retentionLabels().post(requestBody);


```