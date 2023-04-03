---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RetentionLabel();
requestBody.set@odatatype('#microsoft.graph.security.retentionLabel');

retentionDuration = RetentionDuration();
retentionDuration.set@odatatype('microsoft.graph.security.retentionDuration');


requestBody.setRetentionDuration($retentionDuration);
requestBody.setDescriptionForAdmins('String');

requestBody.setDescriptionForUsers('String');

requestBody.setLabelToBeApplied('String');

requestBody.setDefaultRecordBehavior(DefaultRecordBehavior('string'));



result = await client.security().labels().retentionLabelsById('retentionLabel-id').patch(requestBody);


```