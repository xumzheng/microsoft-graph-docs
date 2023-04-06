---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GenerateKeyPostRequestBody()
request_body.setUse('sig')

request_body.setKty('RSA')

request_body.setNbf(1508969811)

request_body.setExp(1508969811)


request_config = GenerateKeyRequestBuilderPostRequestConfiguration(
request_config = GenerateKeyRequestBuilderPostRequestConfiguration(query_params=)


result = await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').generateKey.post(request_body, headers=)


```