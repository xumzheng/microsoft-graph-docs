---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Continuous_access_evaluation_policy()
request_body.@odata_type = '#microsoft.graph.continuousAccessEvaluationPolicy'

request_body.migrate = True




result = await client.identity.continuou_acces_evaluation_policy.patch(request_body = request_body)


```