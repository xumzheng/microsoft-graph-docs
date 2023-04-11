---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionLabel()
request_body.@odatatype = '#microsoft.graph.security.retentionLabel'

request_body.displayName = 'String'

request_body.BehaviorDuringRetentionPeriod(BehaviorDuringRetentionPeriod('string'))

request_body.ActionAfterRetentionPeriod(ActionAfterRetentionPeriod('string'))

request_body.RetentionTrigger(RetentionTrigger('string'))

retentionDuration = RetentionDuration()
retentionDuration.@odatatype = 'microsoft.graph.security.retentionDuration'


request_body.retentionDuration = retentionDuration
request_body.isInUse = boolean

request_body.descriptionForAdmins = 'String'

request_body.descriptionForUsers = 'String'

createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy
request_body.labelToBeApplied = 'String'

request_body.DefaultRecordBehavior(DefaultRecordBehavior('string'))




result = await client.security.labels.retentionLabels.post(request_body = request_body)


```