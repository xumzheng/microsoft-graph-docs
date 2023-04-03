---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TranslateExchangeIdsPostRequestBody();
requestBody.setInputIds(['{rest-formatted-id-1}', '{rest-formatted-id-2}', ]);

requestBody.setSourceIdType(ExchangeIdFormat('restid'));

requestBody.setTargetIdType(ExchangeIdFormat('restimmutableentryid'));



result = await client.me().translateExchangeIds().post(requestBody);


```