---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.setDescription('Contoso Life v2.0')

request_body.setDisplayName('Contoso Life Renewed')



result = await client.groupsById('group-id').patch(request_body)


```