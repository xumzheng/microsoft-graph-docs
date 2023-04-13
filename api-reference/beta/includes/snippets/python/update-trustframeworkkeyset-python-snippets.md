---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = KeySet()
additionalData = [
'keys' => keys1 = ()
		keys1.k = 'k-value'

keys1.X5c(['x5c-value', ])

	keys1.x5t = 'x5t-value'

	keys1.kty = 'kty-value'

	keys1.use = 'use-value'

	keys1.exp = 99

	keys1.nbf = 99

	keys1.kid = 'kid-value'

	keys1.e = 'e-value'

	keys1.n = 'n-value'

	keys1.d = 'd-value'

	keys1.p = 'p-value'

	keys1.q = 'q-value'

	keys1.dp = 'dp-value'

	keys1.dq = 'dq-value'

	keys1.qi = 'qi-value'


keysArray []= keys1;
request_body.keys(keysArray)


];
request_body.additionaldata(additionalData)





await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').put(request_body = request_body)


```