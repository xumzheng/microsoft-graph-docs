---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Notebook()
request_body.displayName = 'My Private notebook'



request_configuration = NotebooksRequestBuilderPostRequestConfiguration(
)


result = await client.me.onenote.notebooks.post(request_body = request_body)


```