---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Program()
request_body.setDisplayName('testprogram3')

request_body.setDescription('test description')



result = await client.programs.post(request_body)


```