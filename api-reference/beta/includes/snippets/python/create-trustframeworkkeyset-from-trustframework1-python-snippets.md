---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TrustFrameworkKeySet()
request_body.id = 'keyset1'



request_configuration = KeySetsRequestBuilderPostRequestConfiguration(
)


result = await client.trustFramework.keySets.post(request_body = request_body)


```