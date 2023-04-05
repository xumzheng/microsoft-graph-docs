---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SitePage()
request_body.set@odatatype('#microsoft.graph.sitePage')

request_body.setTitle('sample')

request_body.setShowComments(true)

request_body.setShowRecommendedPages(false)



result = await client.sitesby_id('site-id')_pagesby_id('sitePage-id').patch(request_body)


```