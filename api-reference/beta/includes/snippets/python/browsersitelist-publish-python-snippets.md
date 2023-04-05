---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PublishPostRequestBody()
request_body.setRevision('1.0')



result = await client.admin.edge.internetExplorerMode.siteListsby_id('browserSiteList-id').publish.post(request_body)


```