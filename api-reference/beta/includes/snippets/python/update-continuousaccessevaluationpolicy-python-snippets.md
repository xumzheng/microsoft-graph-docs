---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContinuousAccessEvaluationPolicy()
request_body.set@odatatype('#microsoft.graph.continuousAccessEvaluationPolicy')

request_body.setMigrate(true)



result = await client.identity.continuousAccessEvaluationPolicy.patch(request_body, headers=)


```