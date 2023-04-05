---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SubjectRightsRequest()
request_body.set@odatatype('#microsoft.graph.subjectRightsRequest')

request_body.setInternalDueDateTime(DateTime('2021-08-30T00:00:00Z'))



result = await client.privacy.subjectRightsRequests._by_id('subjectRightsRequest-id').patch(request_body)


```