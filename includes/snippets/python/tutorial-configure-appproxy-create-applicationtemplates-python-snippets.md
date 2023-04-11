---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InstantiatePostRequestBody()
request_body.displayName = 'Contoso IWA App'




result = await client.applicationTemplates_by_id('applicationTemplate-id').instantiate.post(request_body = request_body)


```