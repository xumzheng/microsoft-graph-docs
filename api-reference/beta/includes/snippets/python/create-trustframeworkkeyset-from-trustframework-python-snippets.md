---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TrustFrameworkKeySet()
request_body.id = 'keyset1'

keysTrustFrameworkKey1 = TrustFrameworkKey()
keysTrustFrameworkKey1.k = 'k-value'

keysTrustFrameworkKey1.X5c(['x5c-value', ])

keysTrustFrameworkKey1.x5t = 'x5t-value'

keysTrustFrameworkKey1.kty = 'kty-value'

keysTrustFrameworkKey1.use = 'use-value'

keysTrustFrameworkKey1.exp = 99

keysTrustFrameworkKey1.nbf = 99

keysTrustFrameworkKey1.kid = 'kid-value'

keysTrustFrameworkKey1.e = 'e-value'

keysTrustFrameworkKey1.n = 'n-value'

keysTrustFrameworkKey1.d = 'd-value'

keysTrustFrameworkKey1.p = 'p-value'

keysTrustFrameworkKey1.q = 'q-value'

keysTrustFrameworkKey1.dp = 'dp-value'

keysTrustFrameworkKey1.dq = 'dq-value'

keysTrustFrameworkKey1.qi = 'qi-value'


keysArray []= keysTrustFrameworkKey1;
request_body.keys(keysArray)





result = await client.trustFramework.keySets.post(request_body = request_body)


```