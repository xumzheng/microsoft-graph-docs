---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Device();
request_body.setAccountEnabled(false);



result = await client.devicesById('device-id').patch(request_body);


```