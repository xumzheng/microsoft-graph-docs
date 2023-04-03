---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TrustFrameworkKeySet();
requestBody.setId('keyset1');



result = await client.trustFramework().keySets().post(requestBody);


```