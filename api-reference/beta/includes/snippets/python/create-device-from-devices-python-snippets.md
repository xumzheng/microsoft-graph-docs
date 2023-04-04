---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Device()
request_body.setAccountEnabled(true)

alternativeSecurityIdsAlternativeSecurityId1 = AlternativeSecurityId()
alternativeSecurityIdsAlternativeSecurityId1.setType(99)

alternativeSecurityIdsAlternativeSecurityId1.setIdentityProvider('identityProvider-value')

alternativeSecurityIdsAlternativeSecurityId1.setKey(base64_decode('base64Y3YxN2E1MWFlYw=='))


alternativeSecurityIdsArray []= alternativeSecurityIdsAlternativeSecurityId1;
request_body.setAlternativeSecurityIds(alternativeSecurityIdsArray)


request_body.setApproximateLastSignInDateTime(DateTime('2016-10-19T10:37:00Z'))

request_body.setDeviceId('deviceId-value')

request_body.setDeviceMetadata('deviceMetadata-value')

request_body.setDeviceVersion(99)



result = await client.devices.post(request_body)


```