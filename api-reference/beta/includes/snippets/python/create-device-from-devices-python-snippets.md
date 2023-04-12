---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
request_body.accountEnabled = true

alternativeSecurityIdsAlternativeSecurityId1 = AlternativeSecurityId()
alternativeSecurityIdsAlternativeSecurityId1.type = 99

alternativeSecurityIdsAlternativeSecurityId1.identityProvider = 'identityProvider-value'

alternativeSecurityIdsAlternativeSecurityId1.Key(base64_decode('base64Y3YxN2E1MWFlYw=='))


alternativeSecurityIdsArray []= alternativeSecurityIdsAlternativeSecurityId1;
request_body.alternativesecurityids(alternativeSecurityIdsArray)


request_body.approximateLastSignInDateTime = DateTime('2016-10-19T10:37:00Z')

request_body.deviceId = 'deviceId-value'

request_body.deviceMetadata = 'deviceMetadata-value'

request_body.deviceVersion = 99




result = await client.devices.post(request_body = request_body)


```