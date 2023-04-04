---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = User();
request_body.setBusinessPhones(['+1 425 555 0109', ]);

request_body.setOfficeLocation('18/2111');



result = await client.me().patch(request_body);


```