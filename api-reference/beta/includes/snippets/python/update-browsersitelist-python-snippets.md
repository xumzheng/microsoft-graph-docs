---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSiteList()
request_body.setDisplayName('Production Site List A')

request_body.setDescription('Production site list for team A')



result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').patch(request_body)


```