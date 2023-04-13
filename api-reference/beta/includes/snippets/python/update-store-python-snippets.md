---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Store()
request_body.defaultLanguageTag = 'en-US'




result = await client.termStore.patch(request_body = request_body)


```