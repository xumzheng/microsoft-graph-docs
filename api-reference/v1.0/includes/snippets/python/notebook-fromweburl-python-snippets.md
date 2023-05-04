---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Get_notebook_from_web_url_post_request_body()
request_body.web_url = 'webUrl value'




result = await client.me.onenote.notebooks.get_notebook_from_web_url.post(request_body = request_body)


```