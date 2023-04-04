---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RetentionLabel()
request_body.set@odatatype('#microsoft.graph.security.retentionLabel')

retentionDuration = RetentionDuration()
retentionDuration.set@odatatype('microsoft.graph.security.retentionDuration')


request_body.setRetentionDuration($retentionDuration)
request_body.setDescriptionForAdmins('String')

request_body.setDescriptionForUsers('String')

request_body.setLabelToBeApplied('String')

request_body.setDefaultRecordBehavior(DefaultRecordBehavior('string'))



result = await client.security.labels.retentionLabelsById('retentionLabel-id').patch(request_body)


```