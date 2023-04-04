---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SynchronizationSecretKeyStringValuePair()
additionalData = [
'value' => value1 = ()
		value1.setKey('BaseAddress')

		value1.setValue('user@domain.com')


valueArray []= value1;
value2 = ()
		value2.setKey('SecretToken')

		value2.setValue('password-value')


valueArray []= value2;
value3 = ()
		value3.setKey('SyncNotificationSettings')

		value3.setValue('{\"Enabled\":false,\"DeleteThresholdEnabled\":false}')


valueArray []= value3;
value4 = ()
		value4.setKey('SyncAll')

		value4.setValue('false')


valueArray []= value4;
request_body.setValue(valueArray)


];
request_body.setAdditionalData(additionalData)




result = await client.servicePrincipalsById('servicePrincipal-id').synchronization.secrets.put(request_body)


```