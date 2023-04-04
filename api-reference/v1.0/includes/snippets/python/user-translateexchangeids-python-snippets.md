---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TranslateExchangeIdsPostRequestBody();
request_body.setInputIds(['{rest-formatted-id-1}', '{rest-formatted-id-2}', ]);

request_body.setSourceIdType(ExchangeIdFormat('restid'));

request_body.setTargetIdType(ExchangeIdFormat('restimmutableentryid'));



result = await client.me.translateExchangeIds.post(request_body);


```