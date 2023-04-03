---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = KeySet();
additionalData = [
'keys' => keys1 = ();
		keys1.setK('k-value');

keys1.setX5c(['x5c-value', ]);

	keys1.setX5t('x5t-value');

	keys1.setKty('kty-value');

	keys1.setUse('use-value');

	keys1.setExp(99);

	keys1.setNbf(99);

	keys1.setKid('kid-value');

	keys1.setE('e-value');

	keys1.setN('n-value');

	keys1.setD('d-value');

	keys1.setP('p-value');

	keys1.setQ('q-value');

	keys1.setDp('dp-value');

	keys1.setDq('dq-value');

	keys1.setQi('qi-value');


keysArray []= keys1;
requestBody.setKeys(keysArray);


];
requestBody.setAdditionalData(additionalData);




graphServiceClient.trustFramework().keySetsById('trustFrameworkKeySet-id').put(requestBody);


```