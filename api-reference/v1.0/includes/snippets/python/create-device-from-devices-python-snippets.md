---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
request_body.account_enabled = False

alternative_security_ids_alternative_security_id1 = AlternativeSecurityId()
alternativeSecurityIdsAlternativeSecurityId1.type = 2

alternativeSecurityIdsAlternativeSecurityId1.Key(base64_decode('base64Y3YxN2E1MWFlYw=='))


alternativeSecurityIdsArray []= alternativeSecurityIdsAlternativeSecurityId1;
request_body.alternativesecurityids(alternativeSecurityIdsArray)


request_body.deviceId = '4c299165-6e8f-4b45-a5ba-c5d250a707ff'

request_body.displayName = 'Test device'

request_body.operatingSystem = 'linux'

request_body.operatingSystemVersion = '1'




result = await client.devices.post(request_body = request_body)


```