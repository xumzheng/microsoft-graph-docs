---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateTiIndicatorsPostRequestBody()
valueTiIndicator1 = TiIndicator()
valueTiIndicator1.id = 'c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4'

valueTiIndicator1.additionalInformation = 'mytest'


valueArray []= valueTiIndicator1;
valueTiIndicator2 = TiIndicator()
valueTiIndicator2.id = 'e58c072b-c9bb-a5c4-34ce-eb69af44fb1e'

valueTiIndicator2.additionalInformation = 'test again'


valueArray []= valueTiIndicator2;
request_body.value(valueArray)





result = await client.security.tiIndicators.updateTiIndicators.post(request_body = request_body)


```