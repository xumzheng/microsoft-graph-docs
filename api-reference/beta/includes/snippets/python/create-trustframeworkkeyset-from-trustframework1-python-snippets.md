---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TrustFrameworkKeySet()
request_body.setId('keyset1')



result = await client.trustFramework.keySets.post(request_body)


```