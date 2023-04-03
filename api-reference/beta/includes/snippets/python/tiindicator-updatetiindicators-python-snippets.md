---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UpdateTiIndicatorsPostRequestBody();
valueTiIndicator1 = TiIndicator();
valueTiIndicator1.setId('c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4');

valueTiIndicator1.setAdditionalInformation('mytest');


valueArray []= valueTiIndicator1;
valueTiIndicator2 = TiIndicator();
valueTiIndicator2.setId('e58c072b-c9bb-a5c4-34ce-eb69af44fb1e');

valueTiIndicator2.setAdditionalInformation('test again');


valueArray []= valueTiIndicator2;
requestBody.setValue(valueArray);




result = awaitclient.security().tiIndicators().updateTiIndicators().post(requestBody);


```