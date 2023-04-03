---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Device();
requestBody.setAccountEnabled(true);

alternativeSecurityIdsAlternativeSecurityId1 = AlternativeSecurityId();
alternativeSecurityIdsAlternativeSecurityId1.setType(99);

alternativeSecurityIdsAlternativeSecurityId1.setIdentityProvider('identityProvider-value');

alternativeSecurityIdsAlternativeSecurityId1.setKey(base64_decode('base64Y3YxN2E1MWFlYw=='));


alternativeSecurityIdsArray []= alternativeSecurityIdsAlternativeSecurityId1;
requestBody.setAlternativeSecurityIds(alternativeSecurityIdsArray);


requestBody.setApproximateLastSignInDateTime(DateTime('2016-10-19T10:37:00Z'));

requestBody.setDeviceId('deviceId-value');

requestBody.setDeviceMetadata('deviceMetadata-value');

requestBody.setDeviceVersion(99);



result = awaitclient.devices().post(requestBody);


```