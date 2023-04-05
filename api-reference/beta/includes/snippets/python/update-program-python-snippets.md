---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Program()
request_body.setDisplayName('testprogram3 new name')



result = await client.programsby_id('program-id').patch(request_body)


```