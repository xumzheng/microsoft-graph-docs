---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTaskFolder()
request_body.setName('Charity work')



result = await client.me_outlook_taskFoldersby_id('outlookTaskFolder-id').patch(request_body)


```