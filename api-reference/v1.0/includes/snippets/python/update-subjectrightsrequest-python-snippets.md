---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SubjectRightsRequest();
requestBody.set@odatatype('#microsoft.graph.subjectRightsRequest');

requestBody.setInternalDueDateTime(DateTime('2021-08-30T00:00:00Z'));



result = awaitclient.privacy().subjectRightsRequestsById('subjectRightsRequest-id').patch(requestBody);


```