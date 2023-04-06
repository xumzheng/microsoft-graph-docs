---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceUpdate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d')


request_config = RefRequestBuilderPutRequestConfiguration(
request_config = RefRequestBuilderPutRequestConfiguration(query_params=)


await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').rubric.ref.put(request_body, headers=)


```