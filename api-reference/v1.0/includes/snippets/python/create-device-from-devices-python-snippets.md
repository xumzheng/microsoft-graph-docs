---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
request_body.setAccountEnabled(false)

alternativeSecurityIdsAlternativeSecurityId1 = AlternativeSecurityId()
alternativeSecurityIdsAlternativeSecurityId1.setType(2)

alternativeSecurityIdsAlternativeSecurityId1.setKey(base64_decode('base64Y3YxN2E1MWFlYw=='))


alternativeSecurityIdsArray []= alternativeSecurityIdsAlternativeSecurityId1;
request_body.setAlternativeSecurityIds(alternativeSecurityIdsArray)


request_body.setDeviceId('4c299165-6e8f-4b45-a5ba-c5d250a707ff')

request_body.setDisplayName('Test device')

request_body.setOperatingSystem('linux')

request_body.setOperatingSystemVersion('1')


request_config = DevicesRequestBuilderPostRequestConfiguration(
request_config = DevicesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.devices.post(request_body, headers=)


```