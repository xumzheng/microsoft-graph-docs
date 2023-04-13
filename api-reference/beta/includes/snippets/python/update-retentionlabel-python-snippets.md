---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionLabel()
request_body.@odatatype = '#microsoft.graph.security.retentionLabel'

retention_duration = RetentionDuration()
retentionDuration.@odatatype = 'microsoft.graph.security.retentionDuration'


request_body.retention_duration = retentionDuration
request_body.descriptionForAdmins = 'String'

request_body.descriptionForUsers = 'String'

request_body.labelToBeApplied = 'String'

request_body.DefaultRecordBehavior(DefaultRecordBehavior('string'))




result = await client.security.labels.retentionLabels_by_id('retentionLabel-id').patch(request_body = request_body)


```