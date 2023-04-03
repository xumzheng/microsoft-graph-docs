---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RetentionEventType();
requestBody.set@odatatype('#microsoft.graph.security.retentionEventType');

requestBody.setDisplayName('String');

requestBody.setDescription('String');

createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);


result = awaitclient.security().triggerTypes().retentionEventTypes().post(requestBody);


```