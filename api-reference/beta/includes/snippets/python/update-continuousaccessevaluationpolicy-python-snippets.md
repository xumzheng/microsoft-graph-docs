---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContinuousAccessEvaluationPolicy()
request_body.@odatatype = '#microsoft.graph.continuousAccessEvaluationPolicy'

request_body.migrate = true




result = await client.identity.continuousAccessEvaluationPolicy.patch(request_body = request_body)


```