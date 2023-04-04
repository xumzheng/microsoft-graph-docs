---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RetentionLabel()
request_body.set@odatatype('#microsoft.graph.security.retentionLabel')

request_body.setDisplayName('String')

request_body.setBehaviorDuringRetentionPeriod(BehaviorDuringRetentionPeriod('string'))

request_body.setActionAfterRetentionPeriod(ActionAfterRetentionPeriod('string'))

request_body.setRetentionTrigger(RetentionTrigger('string'))

retentionDuration = RetentionDuration()
retentionDuration.set@odatatype('microsoft.graph.security.retentionDuration')


request_body.setRetentionDuration($retentionDuration)
request_body.setIsInUse(boolean)

request_body.setDescriptionForAdmins('String')

request_body.setDescriptionForUsers('String')

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)
request_body.setLabelToBeApplied('String')

request_body.setDefaultRecordBehavior(DefaultRecordBehavior('string'))



result = await client.security.labels.retentionLabels.post(request_body)


```