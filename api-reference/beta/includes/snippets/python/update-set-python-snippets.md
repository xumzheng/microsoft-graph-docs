---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Set();
request_body.setDescription('mySet');



result = await client.termStore.setsById('set-id').patch(request_body);


```